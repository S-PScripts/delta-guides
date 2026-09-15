# Is Delta detected? Is Delta a virus?
**tl;dr: The answer to both of these questions is no.**

Below is a full list of permissions from Delta v729 for Android. I got it via ADB, but there are other easier methods. <br>

As you can see, there are a lot. It looks sketchy. However, Roblox from the Play Store has the same permissions except for the one in bold; this is 
the one that you get prompted to allow when you open a new version of Delta for the first time. 
It is used to create the Delta folder; this is where the assets for Delta's UI are kept, 
where settings for Delta itself and some scripts are saved, and auto-execution.

To find this folder, you can use ZArchiver and go to the path: storage/emulated/0

You may use VirusTotal and see it called malware by a vendor or two, but that is just a "false positive" due to the way it works.

As for if it's undetected, that is also a yes... usually. Its UI may be flagged by certain Roblox games, but if you make a report for that, it should get fixed in a new delta update. What happens more often is that a script you execute could get flagged by the Roblox game, but not the Delta client itself. That's not Delta's fault; ask the developer of that script to make it better.

## Priorities
Roblox itself should hopefully not ban you. However, there have been a few ban waves in the past. Sometimes, the ban wave is for many executors, and sometimes it's just for Delta. Due to that, it is advised to use an alt account. Here are some other methods to minimise risk:
- Do not use other executors.
- Do not use fake versions of Delta. The only official/trusted websites are https://deltaexploits.dev and https://deltaexploits.gg, and websites that link from these two.
- Use the latest version of Delta. Remember, the dev team makes pings for updates in the main Delta server (gg/deltax). For iOS users, if Delta is down, don't spoof the version with Ksign/Esign/Feather etc.
- Do not bypass the keysystem, not even once. Make sure you have no keysystem bypass apps on your phone, too.
- You should not use unknown scripts. In uncommon situations, scripts could cause Roblox itself to flag you, not just the game. NOTE: Raknet desync can cause bans!
- You should not exploit during Roblox events. Roblox has made anti-cheat updates during some of them before.
- Do not use fflags (ones offered by tools like BloxStrap or VoidStrap).
- Don't use auto-farming scripts/bots
If you get banned, Roblox will NOT accept your appeals.

## requested permissions:
- android.permission.POST_NOTIFICATIONS
- android.permission.VIBRATE
- com.android.vending.BILLING
- android.permission.INTERNET
- android.permission.ACCESS_NETWORK_STATE
- android.permission.ACCESS_WIFI_STATE
- android.permission.MODIFY_AUDIO_SETTINGS
- android.permission.READ_CONTACTS
- android.permission.USE_FULL_SCREEN_INTENT
- android.permission.DISABLE_KEYGUARD
- **android.permission.MANAGE_EXTERNAL_STORAGE**
- android.permission.RECORD_AUDIO
- android.permission.CAMERA
- com.google.android.gms.permission.AD_ID
- android.permission.DETECT_SCREEN_CAPTURE
- android.permission.USE_BIOMETRIC
- android.permission.USE_FINGERPRINT
- android.permission.ACCESS_ADSERVICES_ATTRIBUTION
- com.samsung.android.mapsagent.permission.READ_APP_INFO
- com.huawei.appmarket.service.commondata.permission.GET_COMMON_DATA
- android.permission.WAKE_LOCK
- android.permission.RECEIVE_BOOT_COMPLETED
- com.google.android.c2dm.permission.RECEIVE
- com.google.android.finsky.permission.BIND_GET_INSTALL_REFERRER_SERVICE
- android.permission.ACCESS_ADSERVICES_AD_ID
- com.roblox.client.DYNAMIC_RECEIVER_NOT_EXPORTED_PERMISSION
- android.permission.READ_BASIC_PHONE_STATE
- android.permission.ACCESS_ADSERVICES_TOPICS
## install permissions:
- com.google.android.finsky.permission.BIND_GET_INSTALL_REFERRER_SERVICE: granted=true

## Other notes:
- Please remember that despite our claims, we CANNOT guarantee it will always be undetected. It can still occasionally be.
- If you get detected, delete your delta and reinstall it. Once you've done that, DO NOT use that account for at least 2 weeks (assuming it's a warn/1d/7d ban).

- REGARDING BANWAVES: If you get banned, it was NOT from the latest version. It was an exploiting flag from an older version that was only applied later. The latest version of Delta is likely safe.
- Although most exploiting bans are given in ban waves, that doesn't mean it's always like that. When it's not in a ban wave, it is usually not because of Delta.
