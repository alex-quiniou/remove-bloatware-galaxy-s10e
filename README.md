# Bloatware remover for | Galaxy S10e Android 11 (SM-G970F/DS)

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

1. Download and unzip [Minimal ADB and Fastboot (portable version --> zip)](https://forum.xda-developers.com/showthread.php?t=2317790)
    1. After dowloaded ***Minimal ADB and Fastboot***, unzip it where you want
    2. Double click on ***cmd-here.exe***
    3. Type inside CMD window ***adb devices***, it will launch daemon (*daemon not running; *starting now at tcp:5037 * daemon started successfully)
2. [Enable developer options](https://developer.android.com/studio/debug/dev-options#enable)
    1. Settings > About Phone > Information about software > Build Number
    2. Poque it more than 7 times
    3. It will say ***developper mode has been activated***
3. [Enable USB debugging](https://developer.android.com/studio/debug/dev-options#enable)
    1. Go back twice
    2. Inside the parameter app, at the bottom clic at ***developpers options***
    3. Find and toggle ***USB Debugging***
4. Connect your phone to your PC
    1. On your phone autorize ***Autorize phone debugging*** and check ***Always autorize this computer***
5. Check your device connectivity
    1. type ***adb devices*** ,you should see after ***List of devices attached*** your phone with random letters and numbers before the word ***device***
6. Shell
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
pm uninstall -k --user 0 'com.samsung.android.bixby.wakeup'  
pm uninstall -k --user 0 'com.samsung.android.bixby.agent.dummy'  
pm uninstall -k --user 0 '[com.samsung.android.app.routines](http://apps.samsung.com/appquery/appDetail.as?appId=com.samsung.android.app.routines&cId=000004770242)'  
pm uninstall -k --user 0 'com.samsung.android.visionintelligence'  

### Knox
pm uninstall -k --user 0 'com.samsung.android.knox.containercore'  
pm uninstall -k --user 0 'com.samsung.android.knox.attestation'  
pm uninstall -k --user 0 'com.samsung.android.knox.containeragent'  
pm uninstall -k --user 0 'com.samsung.android.knox.pushmanager'  
pm uninstall -k --user 0 'com.samsung.android.knox.analytics.uploader'  
pm uninstall -k --user 0 'com.samsung.android.bbc.bbcagent'  
pm uninstall -k --user 0 'com.samsung.knox.keychain'  
pm uninstall -k --user 0 'com.samsung.knox.securefolder'  
pm uninstall -k --user 0 'com.knox.vpn.proxyhandler'  
pm uninstall -k --user 0 'com.sec.enterprise.knox.cloudmdm.smdms'  
pm uninstall -k --user 0 'com.sec.enterprise.knox.attestation'  

### Dex
pm uninstall -k --user 0 'com.sec.android.app.dexonpc'  
pm uninstall -k --user 0 'com.sec.android.app.desktoplauncher'  
pm uninstall -k --user 0 'com.samsung.desktopsystemui'  
pm uninstall -k --user 0 'com.sec.android.desktopmode.uiservice'  

### Samsung Smart Switch Mobile
pm uninstall -k --user 0 'com.samsung.android.smartswitchassistant'  
pm uninstall -k --user 0 'com.sec.android.easyMover.Agent'  

### Samsung Pass(word autofill)
pm uninstall -k --user 0 'com.samsung.android.samsungpassautofill'  
pm uninstall -k --user 0 'com.samsung.android.samsungpass'  
pm uninstall -k --user 0 'com.samsung.android.authfw'  

### Galaxy Theme app administrator
pm uninstall -k --user 0 'com.samsung.android.themestore'  
pm uninstall -k --user 0 'com.samsung.android.themecenter'  

### Galaxy Theme styles
pm uninstall -k --user 0 'com.android.theme.color.cinnamon'  
pm uninstall -k --user 0 'com.android.theme.color.black'  
pm uninstall -k --user 0 'com.android.theme.color.green'  
pm uninstall -k --user 0 'com.android.theme.color.ocean'  
pm uninstall -k --user 0 'com.android.theme.color.space'  
pm uninstall -k --user 0 'com.android.theme.color.orchid'  
pm uninstall -k --user 0 'com.android.theme.color.purple'  
pm uninstall -k --user 0 'com.android.theme.icon_pack.rounded.systemui'  
pm uninstall -k --user 0 'com.android.theme.icon_pack.rounded.android'  
pm uninstall -k --user 0 'com.android.theme.icon_pack.circular.themepicker'  
pm uninstall -k --user 0 'com.android.theme.icon_pack.rounded.launcher'  
pm uninstall -k --user 0 'com.android.theme.icon_pack.filled.settings'  
pm uninstall -k --user 0 'com.android.theme.icon_pack.circular.settings'  
pm uninstall -k --user 0 'com.android.theme.icon_pack.filled.systemui'  
pm uninstall -k --user 0 'com.android.theme.icon_pack.filled.android'  
pm uninstall -k --user 0 'com.android.theme.icon_pack.circular.systemui'  
pm uninstall -k --user 0 'com.android.theme.icon_pack.filled.launcher'  
pm uninstall -k --user 0 'com.android.theme.icon_pack.circular.launcher'  
pm uninstall -k --user 0 'com.android.theme.icon_pack.filled.themepicker'  
pm uninstall -k --user 0 'com.android.theme.icon_pack.rounded.settings'  
pm uninstall -k --user 0 'com.android.theme.icon_pack.circular.android'  
pm uninstall -k --user 0 'com.android.theme.icon_pack.rounded.themepicker'  
pm uninstall -k --user 0 'com.android.theme.icon.teardrop'  
pm uninstall -k --user 0 'com.android.theme.icon.squircle'  
pm uninstall -k --user 0 'com.android.theme.icon.roundedrect'  
pm uninstall -k --user 0 'com.android.theme.icon.pebble'  
pm uninstall -k --user 0 'com.android.theme.icon.vessel'  
pm uninstall -k --user 0 'com.android.theme.icon.taperedrect'  
pm uninstall -k --user 0 'com.android.theme.font.notoserifsource'  

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
pm uninstall -k --user 0 'com.sec.android.app.clockpackage'  

### Samsung Games
pm uninstall -k --user 0 'com.samsung.android.game.gamehome'  
pm uninstall -k --user 0 'com.samsung.android.game.gametools'  
pm uninstall -k --user 0 'com.samsung.android.game.gos'  
pm uninstall -k --user 0 'com.samsung.gamedriver.ex9820'  

### Samsung AR
pm uninstall -k --user 0 'com.samsung.android.aremoji'  
pm uninstall -k --user 0 'com.samsung.android.ardrawing'  
pm uninstall -k --user 0 'com.samsung.android.app.camera.sticker.facearavatar.preload'  
pm uninstall -k --user 0 'com.samsung.android.arzone'  
pm uninstall -k --user 0 'com.samsung.android.livestickers'  
pm uninstall -k --user 0 'com.samsung.android.hmt.vrsvc'  

### Samsung Share apps
pm uninstall -k --user 0 'com.samsung.android.app.simplesharing'  
pm uninstall -k --user 0 'com.samsung.android.aware.service'  
pm uninstall -k --user 0 'com.samsung.android.app.sharelive'  
pm uninstall -k --user 0 'com.samsung.android.privateshare'  

### Lateral Panel
pm uninstall -k --user 0 'com.samsung.android.app.clipboardedge'  
pm uninstall -k --user 0 'com.sec.android.app.quicktool'  
pm uninstall -k --user 0 'com.samsung.android.mdx.quickboard'  
pm uninstall -k --user 0 'com.samsung.android.app.cocktailbarservice'  
pm uninstall -k --user 0 'package:com.samsung.android.app.appsedge'  
pm uninstall -k --user 0 'package:com.samsung.android.app.taskedge'  

# 3. Hard list removal
You are probably using one of them. Pay attention about your actions !

### Microsoft
| Syntax      | App Name `FRENCH / ENGLISH` | what this app do ? |
| ----------- | ----------- | ----------- |
| pm uninstall -k --user 0 '[com.microsoft.skydrive](https://play.google.com/store/apps/details?id=com.microsoft.skydrive)' | Microsoft OneDrive | See Play Store |
| pm uninstall -k --user 0 '[com.microsoft.appmanager](https://play.google.com/store/apps/details?id=com.microsoft.appmanager)' | Your Phone Companion - Link to Windows | See Play Store |

### Google
| Syntax      | App Name `FRENCH / ENGLISH` | what this app do ? |
| ----------- | ----------- | ----------- |
| pm uninstall -k --user 0 '[com.android.chrome](https://play.google.com/store/apps/details?id=com.android.chrome)' | Google Chrome: Fast & Secure | See Play Store |
| pm uninstall -k --user 0 '[com.google.android.youtube](https://play.google.com/store/apps/details?id=com.google.android.youtube)' | YouTube | See Play Store |
| pm uninstall -k --user 0 '[com.google.android.googlequicksearchbox](https://play.google.com/store/apps/details?id=com.google.android.googlequicksearchbox)' | Google | See Play Store |
| pm uninstall -k --user 0 '[com.google.ar.core](https://play.google.com/store/apps/details?id=com.google.ar.core)' | Google Play Services for AR | See Play Store |
| pm uninstall -k --user 0 '[com.google.android.gm](https://play.google.com/store/apps/details?id=com.google.android.gm)' | Gmail | See Play Store |
| pm uninstall -k --user 0 '[com.google.android.music](https://play.google.com/store/apps/details?id=com.google.android.music)' | Google Play Music | See Play Store |
| pm uninstall -k --user 0 '[com.google.android.apps.docs](https://play.google.com/store/apps/details?id=com.google.android.apps.docs)' | Google Drive | See Play Store |
| pm uninstall -k --user 0 '[com.google.android.apps.maps](https://play.google.com/store/apps/details?id=com.google.android.apps.maps)' | Maps - Navigate & Explore | See Play Store |
| pm uninstall -k --user 0 '[com.google.android.tts](https://play.google.com/store/apps/details?id=com.google.android.tts)' | Google Text-to-Speech | See Play Store |
| pm uninstall -k --user 0 '[com.google.android.videos](https://play.google.com/store/apps/details?id=com.google.android.videos)' | Google Play Movies & TV | See Play Store |
| pm uninstall -k --user 0 '[com.google.android.apps.photos](https://play.google.com/store/apps/details?id=com.google.android.apps.photos)' | Google Photos | See Play Store |
| pm uninstall -k --user 0 '[com.google.android.apps.turbo](https://play.google.com/store/apps/details?id=com.google.android.apps.turbo)' | Device Health Services | See Play Store |
| pm uninstall -k --user 0 '[com.google.android.gms](https://play.google.com/store/apps/details?id=com.google.android.gms)' | Services Google Play | See Play Store |
| pm uninstall -k --user 0 '[com.google.android.webview](https://play.google.com/store/apps/details?id=com.google.android.webview)' | Android System WebView | See Play Store |
| pm uninstall -k --user 0 '[com.google.android.as](https://play.google.com/store/apps/details?id=com.google.android.as)' | Services de personnalisation de l'appareil | See Play Store |
| pm uninstall -k --user 0 '[com.google.android.projection.gearhead](https://play.google.com/store/apps/details?id=com.google.android.projection.gearhead)' | Android Auto - Google Maps, Media & Messaging | See Play Store |
| pm uninstall -k --user 0 '[com.google.android.apps.tachyon](https://play.google.com/store/apps/details?id=com.google.android.apps.tachyon)' | Google Duo - High Quality Video Calls | See Play Store |
| ----------- | ----------- | ----------- |
| pm uninstall -k --user 0 'com.google.android.gms.location.history' | Historique des positions Google | ***HELP NEEDEED*** |
| pm uninstall -k --user 0 'com.google.android.ext.services' | Android Services Library | ***HELP NEEDEED*** |
| pm uninstall -k --user 0 'com.google.android.onetimeinitializer' | Google One Time Init | ***HELP NEEDEED*** |
| pm uninstall -k --user 0 'com.google.android.ext.shared' | Android Shared Library | ***HELP NEEDEED*** |
| pm uninstall -k --user 0 'com.google.android.configupdater' | ConfigUpdater | ***HELP NEEDEED*** |
| pm uninstall -k --user 0 'com.google.android.overlay.modules.permissioncontroller' | - | ***HELP NEEDEED*** |
| pm uninstall -k --user 0 'com.google.android.permissioncontroller' | Contrôleur autorisations | ***HELP NEEDEED*** |
| pm uninstall -k --user 0 'com.google.android.setupwizard' | Configuration d'Android | ***HELP NEEDEED*** |
| pm uninstall -k --user 0 'com.google.android.modulemetadata' | Main components | ***HELP NEEDEED*** |
| pm uninstall -k --user 0 'com.google.android.syncadapters.contacts' | Synchronisation de Google Contacts | ***HELP NEEDEED*** |
| pm uninstall -k --user 0 'com.google.android.packageinstaller' | Programme installation kit | ***HELP NEEDEED*** |
| pm uninstall -k --user 0 'com.google.android.gsf' | Framework des services Google | ***HELP NEEDEED*** |
| pm uninstall -k --user 0 'com.google.android.partnersetup' | Google Partner Setup | ***HELP NEEDEED*** |
| pm uninstall -k --user 0 'com.google.android.feedback' | Market Feedback Agent | ***HELP NEEDEED*** |
| pm uninstall -k --user 0 'com.google.android.printservice.recommendation' | Print Service Recommendation Service | ***HELP NEEDEED*** |
| pm uninstall -k --user 0 'com.google.android.overlay.modules.permissioncontroller.forframework' | - | ***HELP NEEDEED*** |
| pm uninstall -k --user 0 'com.google.android.syncadapters.calendar' | Synchronisation de Google Agenda | ***HELP NEEDEED*** |
| pm uninstall -k --user 0 'com.google.android.apps.restore' | Configuration d'Android | ***HELP NEEDEED*** |
| pm uninstall -k --user 0 'com.google.android.overlay.modules.cellbroadcastreceiver' | - | ***HELP NEEDEED*** |
| pm uninstall -k --user 0 'com.google.android.overlay.gmsconfig.common' | - | ***HELP NEEDEED*** |
| pm uninstall -k --user 0 'com.google.android.overlay.gmsconfig.photos' | - | ***HELP NEEDEED*** |
| pm uninstall -k --user 0 'com.google.android.captiveportallogin' | CaptivePortalLogin | ***HELP NEEDEED*** |
| pm uninstall -k --user 0 'com.google.android.overlay.modules.documentsui' | - | ***HELP NEEDEED*** |
| pm uninstall -k --user 0 'com.google.android.networkstack' | Gestionnaire de réseaux | ***HELP NEEDEED*** |
| pm uninstall -k --user 0 'com.google.android.overlay.gmsconfig.gsa' | - | ***HELP NEEDEED*** |
| pm uninstall -k --user 0 'com.google.android.documentsui' | Fichiers | ***HELP NEEDEED*** |
| pm uninstall -k --user 0 'com.google.mainline.telemetry' | Supports components | ***HELP NEEDEED*** |
| pm uninstall -k --user 0 'com.google.android.networkstack.permissionconfig' | - | ***HELP NEEDEED*** |
| pm uninstall -k --user 0 'com.google.android.overlay.modules.cellbroadcastservice' | - | ***HELP NEEDEED*** |
| pm uninstall -k --user 0 'com.google.android.apps.carrier.carrierwifi' | Google Wi-Fi Provisioner | ***HELP NEEDEED*** |
| pm uninstall -k --user 0 'com.android.hotwordenrollment.okgoogle' | Google Assistant | ***HELP NEEDEED*** |
| pm uninstall -k --user 0 'com.android.hotwordenrollment.xgoogle' | Google Assistant | ***HELP NEEDEED*** |

### Samsung
| Syntax      | App Name `FRENCH / ENGLISH` | what this app do ? |
| ----------- | ----------- | ----------- |
| pm uninstall -k --user 0 '[com.sec.android.app.myfiles](https://play.google.com/store/apps/details?id=com.sec.android.app.myfiles)' | Samsung My Files | See Play Store |
| pm uninstall -k --user 0 '[com.sec.android.gallery3d](https://play.google.com/store/apps/details?id=com.sec.android.gallery3d)' | Samsung Gallery | See Play Store |
| pm uninstall -k --user 0 '[com.samsung.android.app.aodservice](https://play.google.com/store/apps/details?id=com.samsung.android.app.aodservice)' | Always On Display | See Play Store |
| pm uninstall -k --user 0 '[com.samsung.android.lool](https://play.google.com/store/apps/details?id=com.samsung.android.lool)' | Device Care | See Play Store |
| ----------- | ----------- | ----------- |
| pm uninstall -k --user 0 'com.samsung.android.dynamiclock' | Services de fond d'écran | feature for the lock screen |
| pm uninstall -k --user 0 'com.samsung.android.ipsgeofence' | Samsung Visit in | add a banner add notification when it things you are near a samsung store |
| pm uninstall -k --user 0 'com.samsung.android.fast' | Secure Wi-fi | limited VPN offering |
| pm uninstall -k --user 0 'com.samsung.android.mobileservice' | Samsung Experience Service / Group Sharing | ***HELP NEEDEED*** |
| pm uninstall -k --user 0 'com.samsung.android.calendar' | Calendrier | ***HELP NEEDEED*** |
| pm uninstall -k --user 0 'com.sec.android.inputmethod' | Clavier Samsung (obsolète)| ***HELP NEEDEED*** |
| pm uninstall -k --user 0 'com.osp.app.signin' | Compte Samsung | ***HELP NEEDEED*** |
| pm uninstall -k --user 0 'com.samsung.android.app.contacts' | Contacts | ***HELP NEEDEED*** |
| pm uninstall -k --user 0 'com.samsung.android.forest' | Bien-etre numérique et controles parentaux | ***HELP NEEDEED*** |
| pm uninstall -k --user 0 'com.sec.android.app.samsungapps' | Galaxy Store | ***HELP NEEDEED*** |
| pm uninstall -k --user 0 'com.samsung.android.video' | Lecteur vidéo | ***HELP NEEDEED*** |
| pm uninstall -k --user 0 'com.samsung.android.messaging' | Messages | ***HELP NEEDEED*** |
| pm uninstall -k --user 0 'com.samsung.android.wallpaper.res' | com.samsung.android.wallpaper.res | ***HELP NEEDEED*** |
| pm uninstall -k --user 0 'com.samsung.app.newtrim' | Découpage de vidéos | ***HELP NEEDEED*** |
| pm uninstall -k --user 0 'com.samsung.app.highlightplayer' | Créer un film | ***HELP NEEDEED*** |
| pm uninstall -k --user 0 'com.samsung.storyservice' | Histoire de la Galerie | ***HELP NEEDEED*** |
| pm uninstall -k --user 0 'com.samsung.android.service.livedrawing' | Messages animés | ***HELP NEEDEED*** |
| pm uninstall -k --user 0 'com.samsung.android.kidsinstaller' | Programme d'installation Espace enfants | ***HELP NEEDEED*** |
| pm uninstall -k --user 0 'com.samsung.android.svoiceime' | Saisie vocale Samsung | ***HELP NEEDEED*** |
| pm uninstall -k --user 0 'com.samsung.android.app.reminder' | Reminder | ***HELP NEEDEED*** |
| pm uninstall -k --user 0 'com.samsung.android.scloud' | Samsung Cloud | ***HELP NEEDEED*** |
| pm uninstall -k --user 0 'com.samsung.android.app.spage' | Samsung Daily Beta | ***HELP NEEDEED*** |
| pm uninstall -k --user 0 'com.samsung.android.app.tips' | Astuces | ***HELP NEEDEED*** |
| pm uninstall -k --user 0 'com.samsung.android.mdx' | Service Lien avec Windows | ***HELP NEEDEED*** |
| pm uninstall -k --user 0 'com.sec.android.autodoodle.service' | AutoDoodle | ***HELP NEEDEED*** |
| pm uninstall -k --user 0 'com.samsung.android.app.smartcapture' | Capture Samsung | ***HELP NEEDEED*** |
| pm uninstall -k --user 0 'com.samsung.android.honeyboard' | Clavier Samsung | ***HELP NEEDEED*** |
| pm uninstall -k --user 0 'com.sec.android.mimage.photoretouching' | Editeur de photos | ***HELP NEEDEED*** |
| pm uninstall -k --user 0 'com.samsung.android.mateagent' | Samsung Galaxy Friends | ***HELP NEEDEED*** |
| pm uninstall -k --user 0 'com.samsung.android.digitalkey' | Samsung Digital Key | https://global-carconnectivity.org/ |
| pm uninstall -k --user 0 'com.sec.android.daemonapp' | Météo | ***HELP NEEDEED*** |
| pm uninstall -k --user 0 'com.samsung.android.smartmirroring' | Smart View | ***HELP NEEDEED*** |
| pm uninstall -k --user 0 'com.samsung.android.app.watchmanagerstub' | Wearable Manager Installer | ***HELP NEEDEED*** |
| pm uninstall -k --user 0 'com.android.managedprovisioning' | Configuration du profil professionnel | ***HELP NEEDEED*** |
| ----------- | ----------- | ----------- |
| pm uninstall -k --user 0 '[com.sec.android.app.launcher](https://play.google.com/store/apps/details?id=com.sec.android.app.launcher)' | Samsung One UI Home ***WARNING without this no task manager*** | See Play Store |
| pm uninstall -k --user 0 'com.samsung.android.app.galaxyfinder' | Finder ***WARNING without this no search bar in parameter*** | ***HELP NEEDEED*** |

### Other (Help needeed)
| Syntax      | App Name `FRENCH / ENGLISH` | what this app do ? |
| ----------- | ----------- | ----------- |
| pm uninstall -k --user 0 'com.samsung.android.provider.filterprovider' | ***HELP NEEDEED*** | ***HELP NEEDEED*** |
| pm uninstall -k --user 0 'com.sec.android.app.DataCreate' | ***HELP NEEDEED*** | ***HELP NEEDEED*** |
| pm uninstall -k --user 0 'com.android.cts.priv.ctsshim' | ***HELP NEEDEED*** | ***HELP NEEDEED*** |
| pm uninstall -k --user 0 'com.sec.android.widgetapp.samsungapps' | ***HELP NEEDEED*** | ***HELP NEEDEED*** |
| pm uninstall -k --user 0 'com.sec.vsim.ericssonnsds.webapp' | ***HELP NEEDEED*** | ***HELP NEEDEED*** |
| pm uninstall -k --user 0 'com.sec.android.app.setupwizardlegalprovider' | ***HELP NEEDEED*** | ***HELP NEEDEED*** |
| pm uninstall -k --user 0 'com.sec.location.nsflp2' | ***HELP NEEDEED*** | ***HELP NEEDEED*** |
| pm uninstall -k --user 0 'com.sec.android.app.chromecustomizations' | ***HELP NEEDEED*** | ***HELP NEEDEED*** |
| pm uninstall -k --user 0 'com.samsung.android.app.cocktailbarservice' | ***HELP NEEDEED*** | ***HELP NEEDEED*** |
| pm uninstall -k --user 0 'com.android.internal.display.cutout.emulation.corner' | ***HELP NEEDEED*** | ***HELP NEEDEED*** |
| pm uninstall -k --user 0 'com.android.internal.display.cutout.emulation.double' | ***HELP NEEDEED*** | ***HELP NEEDEED*** |
| pm uninstall -k --user 0 'com.samsung.android.beyond.p00.wallpapermulti' | ***HELP NEEDEED*** | ***HELP NEEDEED*** |
| pm uninstall -k --user 0 'com.android.providers.telephony' | ***HELP NEEDEED*** | ***HELP NEEDEED*** |
| pm uninstall -k --user 0 'com.sec.android.app.ve.vebgm' | ***HELP NEEDEED*** | ***HELP NEEDEED*** |
| pm uninstall -k --user 0 'com.sec.android.app.parser' | ***HELP NEEDEED*** | ***HELP NEEDEED*** |
| pm uninstall -k --user 0 'com.android.dynsystem' | ***HELP NEEDEED*** | ***HELP NEEDEED*** |
| pm uninstall -k --user 0 'com.samsung.internal.systemui.navbar.gestural_no_hint_wide_back' | ***HELP NEEDEED*** | ***HELP NEEDEED*** |
| pm uninstall -k --user 0 'com.samsung.android.networkstack' | ***HELP NEEDEED*** | ***HELP NEEDEED*** |
| pm uninstall -k --user 0 'com.samsung.android.timezone.updater' | ***HELP NEEDEED*** | ***HELP NEEDEED*** |
| pm uninstall -k --user 0 'com.android.providers.calendar' | ***HELP NEEDEED*** | ***HELP NEEDEED*** |
| pm uninstall -k --user 0 'com.samsung.clipboardsaveservice' | ***HELP NEEDEED*** | ***HELP NEEDEED*** |
| pm uninstall -k --user 0 'com.sec.automation' | ***HELP NEEDEED*** | ***HELP NEEDEED*** |
| pm uninstall -k --user 0 'com.android.providers.media' | ***HELP NEEDEED*** | ***HELP NEEDEED*** |
| pm uninstall -k --user 0 'com.android.internal.systemui.navbar.gestural_wide_back' | ***HELP NEEDEED*** | ***HELP NEEDEED*** |
| pm uninstall -k --user 0 'com.android.wallpapercropper' | ***HELP NEEDEED*** | ***HELP NEEDEED*** |
| pm uninstall -k --user 0 'com.skms.android.agent' | ***HELP NEEDEED*** | ***HELP NEEDEED*** |
| pm uninstall -k --user 0 'com.samsung.android.mapsagent' | ***HELP NEEDEED*** | ***HELP NEEDEED*** |
| pm uninstall -k --user 0 'com.sec.android.app.safetyassurance' | ***HELP NEEDEED*** | ***HELP NEEDEED*** |
| pm uninstall -k --user 0 'com.samsung.android.incallui' | ***HELP NEEDEED*** | ***HELP NEEDEED*** |
| pm uninstall -k --user 0 'com.sec.factory.camera' | ***HELP NEEDEED*** | ***HELP NEEDEED*** |
| pm uninstall -k --user 0 'com.sec.usbsettings' | ***HELP NEEDEED*** | ***HELP NEEDEED*** |
| pm uninstall -k --user 0 'com.samsung.android.easysetup' | ***HELP NEEDEED*** | ***HELP NEEDEED*** |
| pm uninstall -k --user 0 'com.android.externalstorage' | ***HELP NEEDEED*** | ***HELP NEEDEED*** |
| pm uninstall -k --user 0 'com.sec.android.easyonehand' | ***HELP NEEDEED*** | ***HELP NEEDEED*** |
| pm uninstall -k --user 0 'com.sec.factory' | ***HELP NEEDEED*** | ***HELP NEEDEED*** |
| pm uninstall -k --user 0 'com.android.htmlviewer' | ***HELP NEEDEED*** | ***HELP NEEDEED*** |
| pm uninstall -k --user 0 'com.android.companiondevicemanager' | ***HELP NEEDEED*** | ***HELP NEEDEED*** |
| pm uninstall -k --user 0 'com.android.mms.service' | ***HELP NEEDEED*** | ***HELP NEEDEED*** |
| pm uninstall -k --user 0 'com.samsung.android.rubin.app' | ***HELP NEEDEED*** | ***HELP NEEDEED*** |
| pm uninstall -k --user 0 'com.android.providers.downloads' | ***HELP NEEDEED*** | ***HELP NEEDEED*** |
| pm uninstall -k --user 0 'com.wsomacp' | ***HELP NEEDEED*** | ***HELP NEEDEED*** |
| pm uninstall -k --user 0 'com.samsung.faceservice' | ***HELP NEEDEED*** | ***HELP NEEDEED*** |
| pm uninstall -k --user 0 'com.samsung.gpuwatchapp' | ***HELP NEEDEED*** | ***HELP NEEDEED*** |
| pm uninstall -k --user 0 'com.monotype.android.font.foundation' | ***HELP NEEDEED*** | ***HELP NEEDEED*** |
| pm uninstall -k --user 0 'com.sec.android.widgetapp.easymodecontactswidget' | ***HELP NEEDEED*** | ***HELP NEEDEED*** |
| pm uninstall -k --user 0 'com.samsung.android.MtpApplication' | ***HELP NEEDEED*** | ***HELP NEEDEED*** |
| pm uninstall -k --user 0 'com.sec.android.app.factorykeystring' | ***HELP NEEDEED*** | ***HELP NEEDEED*** |
| pm uninstall -k --user 0 'com.sec.android.emergencymode.service' | ***HELP NEEDEED*** | ***HELP NEEDEED*** |
| pm uninstall -k --user 0 'com.sec.android.app.wlantest' | ***HELP NEEDEED*** | ***HELP NEEDEED*** |
| pm uninstall -k --user 0 'com.samsung.android.accessibility.talkback' | ***HELP NEEDEED*** | ***HELP NEEDEED*** |
| pm uninstall -k --user 0 'com.sec.android.smartfpsadjuster' | ***HELP NEEDEED*** | ***HELP NEEDEED*** |
| pm uninstall -k --user 0 'com.sec.epdgtestapp' | ***HELP NEEDEED*** | ***HELP NEEDEED*** |
| pm uninstall -k --user 0 'com.samsung.android.timezone.data_R' | ***HELP NEEDEED*** | ***HELP NEEDEED*** |
| pm uninstall -k --user 0 'com.sec.sve' | ***HELP NEEDEED*** | ***HELP NEEDEED*** |
| pm uninstall -k --user 0 'com.android.providers.downloads.ui' | ***HELP NEEDEED*** | ***HELP NEEDEED*** |
| pm uninstall -k --user 0 'com.android.vending' | ***HELP NEEDEED*** | ***HELP NEEDEED*** |
| pm uninstall -k --user 0 'com.android.pacprocessor' | ***HELP NEEDEED*** | ***HELP NEEDEED*** |
| pm uninstall -k --user 0 'com.android.simappdialog' | ***HELP NEEDEED*** | ***HELP NEEDEED*** |
| pm uninstall -k --user 0 'com.samsung.android.secsoundpicker' | ***HELP NEEDEED*** | ***HELP NEEDEED*** |
| pm uninstall -k --user 0 'com.samsung.internal.systemui.navbar.sec_gestural' | ***HELP NEEDEED*** | ***HELP NEEDEED*** |
| pm uninstall -k --user 0 'com.samsung.android.SettingsReceiver' | ***HELP NEEDEED*** | ***HELP NEEDEED*** |
| pm uninstall -k --user 0 'com.android.internal.display.cutout.emulation.hole' | ***HELP NEEDEED*** | ***HELP NEEDEED*** |
| pm uninstall -k --user 0 'com.android.internal.display.cutout.emulation.tall' | ***HELP NEEDEED*** | ***HELP NEEDEED*** |
| pm uninstall -k --user 0 'com.sec.android.app.soundalive' | ***HELP NEEDEED*** | ***HELP NEEDEED*** |
| pm uninstall -k --user 0 'com.sec.android.provider.badge' | ***HELP NEEDEED*** | ***HELP NEEDEED*** |
| pm uninstall -k --user 0 'com.android.certinstaller' | ***HELP NEEDEED*** | ***HELP NEEDEED*** |
| pm uninstall -k --user 0 'com.samsung.android.securitylogagent' | ***HELP NEEDEED*** | ***HELP NEEDEED*** |
| pm uninstall -k --user 0 'com.android.carrierconfig' | ***HELP NEEDEED*** | ***HELP NEEDEED*** |
| pm uninstall -k --user 0 'com.android.internal.systemui.navbar.threebutton' | ***HELP NEEDEED*** | ***HELP NEEDEED*** |
| pm uninstall -k --user 0 'com.samsung.SMT' | ***HELP NEEDEED*** | ***HELP NEEDEED*** |
| pm uninstall -k --user 0 'com.samsung.cmh' | ***HELP NEEDEED*** | ***HELP NEEDEED*** |
| pm uninstall -k --user 0 'com.samsung.mlp' | ***HELP NEEDEED*** | ***HELP NEEDEED*** |
| pm uninstall -k --user 0 'com.samsung.rcs' | ***HELP NEEDEED*** | ***HELP NEEDEED*** |
| pm uninstall -k --user 0 'android' | ***HELP NEEDEED*** | ***HELP NEEDEED*** |
| pm uninstall -k --user 0 'com.samsung.android.sm.devicesecurity' | ***HELP NEEDEED*** | ***HELP NEEDEED*** |
| pm uninstall -k --user 0 'com.samsung.android.providers.carrier' | ***HELP NEEDEED*** | ***HELP NEEDEED*** |
| pm uninstall -k --user 0 'com.samsung.internal.systemui.navbar.sec_gestural_no_hint' | ***HELP NEEDEED*** | ***HELP NEEDEED*** |
| pm uninstall -k --user 0 'com.samsung.android.aircommandmanager' | ***HELP NEEDEED*** | ***HELP NEEDEED*** |
| pm uninstall -k --user 0 'com.samsung.android.net.wifi.wifiguider' | ***HELP NEEDEED*** | ***HELP NEEDEED*** |
| pm uninstall -k --user 0 'com.samsung.android.smartface' | ***HELP NEEDEED*** | ***HELP NEEDEED*** |
| pm uninstall -k --user 0 'com.android.egg' | ***HELP NEEDEED*** | ***HELP NEEDEED*** |
| pm uninstall -k --user 0 'com.android.mtp' | ***HELP NEEDEED*** | ***HELP NEEDEED*** |
| pm uninstall -k --user 0 'com.android.nfc' | ***HELP NEEDEED*** | ***HELP NEEDEED*** |
| pm uninstall -k --user 0 'com.android.ons' | ***HELP NEEDEED*** | ***HELP NEEDEED*** |
| pm uninstall -k --user 0 'com.android.stk' | ***HELP NEEDEED*** | ***HELP NEEDEED*** |
| pm uninstall -k --user 0 'com.samsung.android.camerasdkservice' | ***HELP NEEDEED*** | ***HELP NEEDEED*** |
| pm uninstall -k --user 0 'com.android.backupconfirm' | ***HELP NEEDEED*** | ***HELP NEEDEED*** |
| pm uninstall -k --user 0 'com.samsung.klmsagent' | ***HELP NEEDEED*** | ***HELP NEEDEED*** |
| pm uninstall -k --user 0 'com.samsung.android.smartfitting' | ***HELP NEEDEED*** | ***HELP NEEDEED*** |
| pm uninstall -k --user 0 'com.sec.android.app.SecSetupWizard' | ***HELP NEEDEED*** | ***HELP NEEDEED*** |
| pm uninstall -k --user 0 'com.samsung.android.app.telephonyui' | ***HELP NEEDEED*** | ***HELP NEEDEED*** |
| pm uninstall -k --user 0 'com.samsung.android.wifi.softap.resources' | ***HELP NEEDEED*** | ***HELP NEEDEED*** |
| pm uninstall -k --user 0 'com.samsung.android.samsungpositioning' | ***HELP NEEDEED*** | ***HELP NEEDEED*** |
| pm uninstall -k --user 0 'com.android.statementservice' | ***HELP NEEDEED*** | ***HELP NEEDEED*** |
| pm uninstall -k --user 0 'com.sec.android.app.hwmoduletest' | ***HELP NEEDEED*** | ***HELP NEEDEED*** |
| pm uninstall -k --user 0 'com.android.settings.intelligence' | ***HELP NEEDEED*** | ***HELP NEEDEED*** |
| pm uninstall -k --user 0 'com.sec.bcservice' | ***HELP NEEDEED*** | ***HELP NEEDEED*** |
| pm uninstall -k --user 0 'com.sec.modem.settings' | ***HELP NEEDEED*** | ***HELP NEEDEED*** |
| pm uninstall -k --user 0 'com.monotype.android.font.samsungone' | ***HELP NEEDEED*** | ***HELP NEEDEED*** |
| pm uninstall -k --user 0 'com.android.internal.systemui.navbar.gestural_extra_wide_back' | ***HELP NEEDEED*** | ***HELP NEEDEED*** |
| pm uninstall -k --user 0 'com.sec.android.app.servicemodeapp' | ***HELP NEEDEED*** | ***HELP NEEDEED*** |
| pm uninstall -k --user 0 'com.sec.android.preloadinstaller' | ***HELP NEEDEED*** | ***HELP NEEDEED*** |
| pm uninstall -k --user 0 'com.samsung.android.tadownloader' | ***HELP NEEDEED*** | ***HELP NEEDEED*** |
| pm uninstall -k --user 0 'com.android.providers.settings' | ***HELP NEEDEED*** | ***HELP NEEDEED*** |
| pm uninstall -k --user 0 'com.samsung.accessibility' | ***HELP NEEDEED*** | ***HELP NEEDEED*** |
| pm uninstall -k --user 0 'com.sec.imsservice' | ***HELP NEEDEED*** | ***HELP NEEDEED*** |
| pm uninstall -k --user 0 'com.android.sharedstoragebackup' | ***HELP NEEDEED*** | ***HELP NEEDEED*** |
| pm uninstall -k --user 0 'com.android.printspooler' | ***HELP NEEDEED*** | ***HELP NEEDEED*** |
| pm uninstall -k --user 0 'com.samsung.android.mdx.kit' | ***HELP NEEDEED*** | ***HELP NEEDEED*** |
| pm uninstall -k --user 0 'com.android.dreams.basic' | ***HELP NEEDEED*** | ***HELP NEEDEED*** |
| pm uninstall -k --user 0 'com.samsung.internal.systemui.navbar.gestural_no_hint_extra_wide_back' | ***HELP NEEDEED*** | ***HELP NEEDEED*** |
| pm uninstall -k --user 0 'com.android.se' | ***HELP NEEDEED*** | ***HELP NEEDEED*** |
| pm uninstall -k --user 0 'com.android.inputdevices' | ***HELP NEEDEED*** | ***HELP NEEDEED*** |
| pm uninstall -k --user 0 'com.samsung.android.wifi.resources' | ***HELP NEEDEED*** | ***HELP NEEDEED*** |
| pm uninstall -k --user 0 'com.android.bips' | ***HELP NEEDEED*** | ***HELP NEEDEED*** |
| pm uninstall -k --user 0 'com.android.stk2' | ***HELP NEEDEED*** | ***HELP NEEDEED*** |
| pm uninstall -k --user 0 'com.samsung.android.cmfa.framework' | ***HELP NEEDEED*** | ***HELP NEEDEED*** |
| pm uninstall -k --user 0 'com.samsung.android.service.peoplestripe' | ***HELP NEEDEED*** | ***HELP NEEDEED*** |
| pm uninstall -k --user 0 'com.samsung.android.da.daagent' | ***HELP NEEDEED*** | ***HELP NEEDEED*** |
| pm uninstall -k --user 0 'com.samsung.android.brightnessbackupservice' | ***HELP NEEDEED*** | ***HELP NEEDEED*** |
| pm uninstall -k --user 0 'com.samsung.android.networkstack.tethering.inprocess.overlay' | ***HELP NEEDEED*** | ***HELP NEEDEED*** |
| pm uninstall -k --user 0 'com.samsung.android.smartcallprovider' | ***HELP NEEDEED*** | ***HELP NEEDEED*** |
| pm uninstall -k --user 0 'com.samsung.advp.imssettings' | ***HELP NEEDEED*** | ***HELP NEEDEED*** |
| pm uninstall -k --user 0 'com.samsung.android.location' | ***HELP NEEDEED*** | ***HELP NEEDEED*** |
| pm uninstall -k --user 0 'com.android.cellbroadcastreceiver' | ***HELP NEEDEED*** | ***HELP NEEDEED*** |
| pm uninstall -k --user 0 'com.sec.android.RilServiceModeApp' | ***HELP NEEDEED*** | ***HELP NEEDEED*** |
| pm uninstall -k --user 0 'com.samsung.android.mdecservice' | ***HELP NEEDEED*** | ***HELP NEEDEED*** |
| pm uninstall -k --user 0 'com.android.server.telecom' | ***HELP NEEDEED*** | ***HELP NEEDEED*** |
| pm uninstall -k --user 0 'com.samsung.crane' | ***HELP NEEDEED*** | ***HELP NEEDEED*** |
| pm uninstall -k --user 0 'com.android.cellbroadcastservice' | ***HELP NEEDEED*** | ***HELP NEEDEED*** |
| pm uninstall -k --user 0 'com.sec.imslogger' | ***HELP NEEDEED*** | ***HELP NEEDEED*** |
| pm uninstall -k --user 0 'com.android.keychain' | ***HELP NEEDEED*** | ***HELP NEEDEED*** |
| pm uninstall -k --user 0 'com.samsung.android.server.wifi.mobilewips' | ***HELP NEEDEED*** | ***HELP NEEDEED*** |
| pm uninstall -k --user 0 'android.autoinstalls.config.samsung' | ***HELP NEEDEED*** | ***HELP NEEDEED*** |
| pm uninstall -k --user 0 'com.android.wifi.resources' | ***HELP NEEDEED*** | ***HELP NEEDEED*** |
| pm uninstall -k --user 0 'com.samsung.android.container' | ***HELP NEEDEED*** | ***HELP NEEDEED*** |
| pm uninstall -k --user 0 'com.android.calllogbackup' | ***HELP NEEDEED*** | ***HELP NEEDEED*** |
| pm uninstall -k --user 0 'com.sec.android.diagmonagent' | ***HELP NEEDEED*** | ***HELP NEEDEED*** |
| pm uninstall -k --user 0 'com.android.localtransport' | ***HELP NEEDEED*** | ***HELP NEEDEED*** |
| pm uninstall -k --user 0 'com.samsung.android.biometrics.app.setting' | ***HELP NEEDEED*** | ***HELP NEEDEED*** |
| pm uninstall -k --user 0 'com.sec.spp.push' | ***HELP NEEDEED*** | ***HELP NEEDEED*** |
| pm uninstall -k --user 0 'com.android.carrierdefaultapp' | ***HELP NEEDEED*** | ***HELP NEEDEED*** |
| pm uninstall -k --user 0 'com.android.proxyhandler' | ***HELP NEEDEED*** | ***HELP NEEDEED*** |
| pm uninstall -k --user 0 'com.android.internal.display.cutout.emulation.waterfall' | ***HELP NEEDEED*** | ***HELP NEEDEED*** |
| pm uninstall -k --user 0 'com.samsung.android.allshare.service.fileshare' | ***HELP NEEDEED*** | ***HELP NEEDEED*** |
| pm uninstall -k --user 0 'com.sec.android.app.apex' | ***HELP NEEDEED*** | ***HELP NEEDEED*** |
| pm uninstall -k --user 0 'com.samsung.sec.android.teegris.tui_service' | ***HELP NEEDEED*** | ***HELP NEEDEED*** |
| pm uninstall -k --user 0 'com.samsung.android.setting.multisound' | ***HELP NEEDEED*** | ***HELP NEEDEED*** |
| pm uninstall -k --user 0 'com.android.dreams.phototable' | ***HELP NEEDEED*** | ***HELP NEEDEED*** |
| pm uninstall -k --user 0 'com.samsung.safetyinformation' | ***HELP NEEDEED*** | ***HELP NEEDEED*** |
| pm uninstall -k --user 0 'com.samsung.android.dialer' | ***HELP NEEDEED*** | ***HELP NEEDEED*** |
| pm uninstall -k --user 0 'com.samsung.android.dqagent' | ***HELP NEEDEED*** | ***HELP NEEDEED*** |
| pm uninstall -k --user 0 'com.sec.android.app.ringtoneBR' | ***HELP NEEDEED*** | ***HELP NEEDEED*** |
| pm uninstall -k --user 0 'com.sec.android.app.vepreload' | ***HELP NEEDEED*** | ***HELP NEEDEED*** |
| pm uninstall -k --user 0 'com.android.providers.partnerbookmarks' | ***HELP NEEDEED*** | ***HELP NEEDEED*** |
| pm uninstall -k --user 0 'com.samsung.internal.systemui.navbar.gestural_no_hint_narrow_back' | ***HELP NEEDEED*** | ***HELP NEEDEED*** |
| pm uninstall -k --user 0 'com.samsung.android.hdmapp' | ***HELP NEEDEED*** | ***HELP NEEDEED*** |
| pm uninstall -k --user 0 'com.sem.factoryapp' | ***HELP NEEDEED*** | ***HELP NEEDEED*** |
| pm uninstall -k --user 0 'com.android.wallpaper.livepicker' | ***HELP NEEDEED*** | ***HELP NEEDEED*** |
| pm uninstall -k --user 0 'com.samsung.android.beaconmanager' | ***HELP NEEDEED*** | ***HELP NEEDEED*** |
| pm uninstall -k --user 0 'com.samsung.internal.systemui.navbar.gestural_no_hint' | ***HELP NEEDEED*** | ***HELP NEEDEED*** |
| pm uninstall -k --user 0 'com.sec.enterprise.mdm.services.simpin' | ***HELP NEEDEED*** | ***HELP NEEDEED*** |
| pm uninstall -k --user 0 'com.android.apps.tag' | ***HELP NEEDEED*** | ***HELP NEEDEED*** |
| pm uninstall -k --user 0 'com.samsung.android.stickercenter' | ***HELP NEEDEED*** | ***HELP NEEDEED*** |
| pm uninstall -k --user 0 'com.samsung.android.providers.media' | ***HELP NEEDEED*** | ***HELP NEEDEED*** |
| pm uninstall -k --user 0 'com.sec.android.soagent' | ***HELP NEEDEED*** | ***HELP NEEDEED*** |
| pm uninstall -k --user 0 'com.samsung.android.fmm' | ***HELP NEEDEED*** | ***HELP NEEDEED*** |
| pm uninstall -k --user 0 'com.samsung.android.mdm' | ***HELP NEEDEED*** | ***HELP NEEDEED*** |
| pm uninstall -k --user 0 'com.samsung.android.scs' | ***HELP NEEDEED*** | ***HELP NEEDEED*** |
| pm uninstall -k --user 0 'com.sec.unifiedwfc' | ***HELP NEEDEED*** | ***HELP NEEDEED*** |
| pm uninstall -k --user 0 'com.sec.phone' | ***HELP NEEDEED*** | ***HELP NEEDEED*** |
| pm uninstall -k --user 0 'com.samsung.android.appseparation' | ***HELP NEEDEED*** | ***HELP NEEDEED*** |
| pm uninstall -k --user 0 'com.android.storagemanager' | ***HELP NEEDEED*** | ***HELP NEEDEED*** |
| pm uninstall -k --user 0 'com.samsung.android.app.soundpicker' | ***HELP NEEDEED*** | ***HELP NEEDEED*** |
| pm uninstall -k --user 0 'com.sec.app.RilErrorNotifier' | ***HELP NEEDEED*** | ***HELP NEEDEED*** |
| pm uninstall -k --user 0 'com.android.bookmarkprovider' | ***HELP NEEDEED*** | ***HELP NEEDEED*** |
| pm uninstall -k --user 0 'com.android.settings' | ***HELP NEEDEED*** | ***HELP NEEDEED*** |
| pm uninstall -k --user 0 'com.samsung.android.dsms' | ***HELP NEEDEED*** | ***HELP NEEDEED*** |
| pm uninstall -k --user 0 'com.sec.android.app.bluetoothtest' | ***HELP NEEDEED*** | ***HELP NEEDEED*** |
| pm uninstall -k --user 0 'com.sec.android.sdhms' | ***HELP NEEDEED*** | ***HELP NEEDEED*** |
| pm uninstall -k --user 0 'com.samsung.android.sm.policy' | ***HELP NEEDEED*** | ***HELP NEEDEED*** |
| pm uninstall -k --user 0 'com.android.networkstack.tethering.inprocess' | ***HELP NEEDEED*** | ***HELP NEEDEED*** |
| pm uninstall -k --user 0 'com.sec.android.emergencylauncher' | ***HELP NEEDEED*** | ***HELP NEEDEED*** |
| pm uninstall -k --user 0 'com.samsung.android.motionphoto.viewer' | ***HELP NEEDEED*** | ***HELP NEEDEED*** |
| pm uninstall -k --user 0 'com.sec.hearingadjust' | ***HELP NEEDEED*** | ***HELP NEEDEED*** |
| pm uninstall -k --user 0 'com.samsung.android.bluelightfilter' | ***HELP NEEDEED*** | ***HELP NEEDEED*** |
| pm uninstall -k --user 0 'com.samsung.android.singletake.service' | ***HELP NEEDEED*** | ***HELP NEEDEED*** |
| pm uninstall -k --user 0 'com.samsung.android.callbgprovider' | ***HELP NEEDEED*** | ***HELP NEEDEED*** |
| pm uninstall -k --user 0 'com.android.cts.ctsshim' | ***HELP NEEDEED*** | ***HELP NEEDEED*** |
| pm uninstall -k --user 0 'com.samsung.android.svcagent' | ***HELP NEEDEED*** | ***HELP NEEDEED*** |
| pm uninstall -k --user 0 'com.sec.mhs.smarttethering' | ***HELP NEEDEED*** | ***HELP NEEDEED*** |
| pm uninstall -k --user 0 'com.samsung.android.networkdiagnostic' | ***HELP NEEDEED*** | ***HELP NEEDEED*** |
| pm uninstall -k --user 0 'com.samsung.android.shortcutbackupservice' | ***HELP NEEDEED*** | ***HELP NEEDEED*** |
| pm uninstall -k --user 0 'com.samsung.android.mcfserver' | ***HELP NEEDEED*** | ***HELP NEEDEED*** |
| pm uninstall -k --user 0 'com.android.vpndialogs' | ***HELP NEEDEED*** | ***HELP NEEDEED*** |
| pm uninstall -k --user 0 'com.samsung.ucs.agent.ese' | ***HELP NEEDEED*** | ***HELP NEEDEED*** |
| pm uninstall -k --user 0 'com.samsung.android.networkstack.tethering.overlay' | ***HELP NEEDEED*** | ***HELP NEEDEED*** |
| pm uninstall -k --user 0 'com.samsung.android.providers.contacts' | ***HELP NEEDEED*** | ***HELP NEEDEED*** |
| pm uninstall -k --user 0 'com.android.phone' | ***HELP NEEDEED*** | ***HELP NEEDEED*** |
| pm uninstall -k --user 0 'com.android.shell' | ***HELP NEEDEED*** | ***HELP NEEDEED*** |
| pm uninstall -k --user 0 'com.android.wallpaperbackup' | ***HELP NEEDEED*** | ***HELP NEEDEED*** |
| pm uninstall -k --user 0 'com.android.providers.blockednumber' | ***HELP NEEDEED*** | ***HELP NEEDEED*** |
| pm uninstall -k --user 0 'com.samsung.android.app.omcagent' | ***HELP NEEDEED*** | ***HELP NEEDEED*** |
| pm uninstall -k --user 0 'com.android.providers.userdictionary' | ***HELP NEEDEED*** | ***HELP NEEDEED*** |
| pm uninstall -k --user 0 'com.android.providers.media.module' | ***HELP NEEDEED*** | ***HELP NEEDEED*** |
| pm uninstall -k --user 0 'com.android.emergency' | ***HELP NEEDEED*** | ***HELP NEEDEED*** |
| pm uninstall -k --user 0 'com.wssyncmldm' | ***HELP NEEDEED*** | ***HELP NEEDEED*** |
| pm uninstall -k --user 0 'com.android.hotspot2.osulogin' | ***HELP NEEDEED*** | ***HELP NEEDEED*** |
| pm uninstall -k --user 0 'com.samsung.ims.smk' | ***HELP NEEDEED*** | ***HELP NEEDEED*** |
| pm uninstall -k --user 0 'com.android.internal.systemui.navbar.gestural' | ***HELP NEEDEED*** | ***HELP NEEDEED*** |
| pm uninstall -k --user 0 'com.android.location.fused' | ***HELP NEEDEED*** | ***HELP NEEDEED*** |
| pm uninstall -k --user 0 'com.sec.epdg' | ***HELP NEEDEED*** | ***HELP NEEDEED*** |
| pm uninstall -k --user 0 'com.android.systemui' | ***HELP NEEDEED*** | ***HELP NEEDEED*** |
| pm uninstall -k --user 0 'com.sec.android.app.personalization' | ***HELP NEEDEED*** | ***HELP NEEDEED*** |
| pm uninstall -k --user 0 'com.sec.factory.cameralyzer' | ***HELP NEEDEED*** | ***HELP NEEDEED*** |
| pm uninstall -k --user 0 'com.android.bluetoothmidiservice' | ***HELP NEEDEED*** | ***HELP NEEDEED*** |
| pm uninstall -k --user 0 'com.samsung.android.sdk.handwriting' | ***HELP NEEDEED*** | ***HELP NEEDEED*** |
| pm uninstall -k --user 0 'com.samsung.aasaservice' | ***HELP NEEDEED*** | ***HELP NEEDEED*** |
| pm uninstall -k --user 0 'com.samsung.android.smartsuggestions' | ***HELP NEEDEED*** | ***HELP NEEDEED*** |
| pm uninstall -k --user 0 'com.android.traceur' | ***HELP NEEDEED*** | ***HELP NEEDEED*** |
| pm uninstall -k --user 0 'com.samsung.android.allshare.service.mediashare' | ***HELP NEEDEED*** | ***HELP NEEDEED*** |
| pm uninstall -k --user 0 'com.samsung.pregpudriver.ex9820' | ***HELP NEEDEED*** | ***HELP NEEDEED*** |
| pm uninstall -k --user 0 'com.sec.android.provider.emergencymode' | ***HELP NEEDEED*** | ***HELP NEEDEED*** |
| pm uninstall -k --user 0 'com.samsung.android.cameraxservice' | ***HELP NEEDEED*** | ***HELP NEEDEED*** |
| pm uninstall -k --user 0 'com.sec.android.app.applinker' | ***HELP NEEDEED*** | ***HELP NEEDEED*** |
| pm uninstall -k --user 0 'com.samsung.android.cidmanager' | ***HELP NEEDEED*** | ***HELP NEEDEED*** |
| pm uninstall -k --user 0 'com.sec.android.app.camera' | ***HELP NEEDEED*** | ***HELP NEEDEED*** |
| pm uninstall -k --user 0 'com.android.bluetooth' | ***HELP NEEDEED*** | ***HELP NEEDEED*** |
| pm uninstall -k --user 0 'com.samsung.ipservice' | ***HELP NEEDEED*** | ***HELP NEEDEED*** |
| pm uninstall -k --user 0 'com.sec.android.app.magnifier' | ***HELP NEEDEED*** | ***HELP NEEDEED*** |
| pm uninstall -k --user 0 'com.sec.android.widgetapp.webmanual' | ***HELP NEEDEED*** | ***HELP NEEDEED*** |
| pm uninstall -k --user 0 'com.samsung.sec.android.application.csc' | ***HELP NEEDEED*** | ***HELP NEEDEED*** |
| pm uninstall -k --user 0 'com.samsung.android.sdm.config' | ***HELP NEEDEED*** | ***HELP NEEDEED*** |
| pm uninstall -k --user 0 'com.samsung.android.app.dressroom' | ***HELP NEEDEED*** | ***HELP NEEDEED*** |
| pm uninstall -k --user 0 'com.android.internal.systemui.navbar.gestural_narrow_back' | ***HELP NEEDEED*** | ***HELP NEEDEED*** |
| pm uninstall -k --user 0 'com.samsung.android.app.dofviewer' | ***HELP NEEDEED*** | ***HELP NEEDEED*** |
| pm uninstall -k --user 0 'com.samsung.android.tapack.authfw' | ***HELP NEEDEED*** | ***HELP NEEDEED*** |
| pm uninstall -k --user 0 'com.samsung.android.bio.face.service' | ***HELP NEEDEED*** | ***HELP NEEDEED*** |
| pm uninstall -k --user 0 'android.auto_generated_rro_vendor__' | ***HELP NEEDEED*** | ***HELP NEEDEED*** |
