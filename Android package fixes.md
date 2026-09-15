# Android Package Fixes

## Errors
1. "App not installed as package appears to be invalid"
2. "App not installed as package conflicts with an existing package"
3. "App not installed as app is not compatible with your phone"
4. "There was a problem parsing the package"
5. "App not installed"

- 1/2/5: Do you already have Roblox or Delta installed? Try deleting them first, then reinstall.
- 1/2/4/5: Install Roblox from the Play Store, then delete it. After that, try to reinstall Delta.
- 1/2/4/5: Are you using the latest version of Android? If not, update it and then reinstall. You should have Android 11 or higher at a minimum.
- 1/2/4/5: Are you downloading it from https://deltaexploits.gg? If not, download and install it from there.
- 1/4/5: Did the APK download fully/correctly? Try re-downloading it using another browser or a VPN.
- 1/2/5: Have you enabled “Allow from unknown sources” for your browser? If not, enable it and try reinstalling.
> Settings > Apps > Special App Access > Install Unknown Apps, select your browser (e.g., Chrome), and toggle Allow from this source.
- 1/2/5: Is Play Protect enabled in the Play Store? Try disabling it, then reinstall.
> Open the Google Play Store app, tap your profile icon, select Play Protect, then Settings (gear icon), and toggle off Scan apps with Play Protect.
- 1/2/5: Do you have multiple profiles or a Secure Folder on your device? Check if Roblox or Delta was installed there.
- 1/4/5: Have you tried to restart your device? Do so, then try to re-install.
- 1/3/4/5: What is your phone’s CPU architecture? (You can use CPU-Z to find out.) If it is ARM32, that might be the issue, since Delta is not supported on ARM32 right now.
- 1/2/4/5: Have you checked if the Roblox folder exists? If not, delete it.
> Install ZArchiver from the Play Store, go to 0/storage/emulated/Android/data, then delete the com.roblox.client folder (if it is there).
- 5: Do you have enough storage? Delete some files you do not need, then try to re-install.
- 1/4/5: Have you tried clearing the cache/data for your package installer?
- 1/4/5: Have you tried using a different package installer (perhaps a file manager's package installer instead of the default one)?

If those don't work, you'll need to use ADB, as it can give more info on what the true problem is: https://rentry.co/delta-package#instructions-no-pc 
(The uninstall command provided is just an example; there are other commands with ADB, like installing APKs that could help fix it).
