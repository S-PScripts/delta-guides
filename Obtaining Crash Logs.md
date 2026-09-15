# Obtaining Crash Logs
Send crash logs to a Delta Support if you are having a problem.

## Android
### ZArchiver Method
1. Install ZArchiver from the Play Store if you do not have it already.
2. Open it, then go to storage/emulated/0.
3. Click the Delta folder, then click the Crashes folder.
4. Send the most recent Crash Log (text) files. You can do this by long-holding a file, clicking Share, then clicking Discord.

### LogFox Method
If there are no files in the Crashes folder, you will have to install LogFox. More information about this app can be found [here](https://github.com/F0x1d/LogFox).

#### Obtaining LogFox
1. Download and install the latest APK for LogFox by clicking [here](https://github.com/F0x1d/LogFox/releases).
2. Install the APK, then open it.
3. If you get a pop-up that says "Permission is required to send notifications with crashes", click OK, then click Allow.
4. You will need to choose one of the options: Root, ADB, or Shizuku. Since you probably do not have any of these three, I will show you how to make ADB work via Termux or Shizuku. I recommend Shizuku, since Termux did not work for me.

#### Obtaining Termux
1. **Enable Developer Mode**
   * Settings → About Phone → tap **Build Number** 7 times
2. **Enable USB Debugging**
   * Developer Options → **USB Debugging → ON**
3. **Install Termux**
   * Go to [F-Droid](https://f-droid.org) and click Download F-Droid. Install the APK.
   * Go back to F-Droid and scroll down to Find Apps.
   * Search for **Termux**, scroll down until you see that exact result, and install it.
4. **Prepare Termux**
   * Open Termux
   *   Update packages:

       ```
       pkg upgrade
       ```
   *   Install ADB tools:

       ```
       pkg install android-tools
       ```
5. **Enable Wireless Debugging**
   * Developer Options → **Wireless Debugging → ON + Allow the connection**
   * Tap **Pair device with pairing code**
   * You need to make sure Termux or Settings is in split view or in a floating window for the next step.
6. **Pair Termux/ADB with Your Device**
   *   In Termux, run:

       ```
       adb pair IP:PAIRING_PORT
       ```

       * Enter the pairing code shown on the phone
   *   Connect to the main port:

       ```
       adb connect IP:MAIN_PORT
       ```
7. In LogFox, click on ADB.
8. If you are on Android 13 or over, it will tell you that you will only be able to see logs for a few minutes before requiring you to restart logging. Click Copy, open Termux, and paste the command. Click Enter.
9. If you get an error, you need to use Shizuku (or use Root (with Termux)).

#### Obtaining Shizuku
1. Download and install the Shizuku APK from [here](https://github.com/RikkaApps/Shizuku/releases/tag/v13.6.0), then open it. You can also use the Play Store, but it was not supported on my phone.
2. Once you open Shizuku, click Pairing. Click "Notification options", then toggle them on. Swipe back, and do what Shizuku tells you to do. Some of the steps are rather similar to the Termux guide above this section, so I will not repeat them.
> Minor note: If you are on OPPO/OnePlus, you will need to _enable_ "Disable permission monitoring" in Developer Options. What Shizuku says is wrong.
3. Once you have Shizuku running, open LogFox and click on Shizuku. Click "Allow all the time" for the "Allow Logfox to access Shizuku?" pop-up. It will close, and when you reopen it, you will be able to see logs appearing. Open Delta, and when you get a crash, it will likely appear in the Crashes section!

## iOS
1. Open the Settings app on your device.
2. Go to Privacy and Security.
3. Click on Analytics and Improvements.
4. Click on Analytic Data; it should be at the top.
5. Find the files that are for Roblox (they start with Roblox). Ensure you find the latest ones (e.g, 2026-07-17 = 17th August 2026).
6. Click on it, then share it with the Delta Support.
