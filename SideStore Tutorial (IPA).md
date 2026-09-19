# Installing Delta via SideStore
**Refer to [https://docs.sidestore.io/docs/troubleshooting/error-codes#apple-developer-errors](https://docs.sidestore.io/docs/troubleshooting/error-codes#apple-developer-errors) for any problems or additional information.** <br />

**If you want to see a different version of this guide, look at the Windows/MacOS/Linux sections here: [https://docs.deltaexploits.gg/installation/ios](https://docs.deltaexploits.gg/installation/ios). The official SideStore docs can be found here: [https://docs.sidestore.io/](https://docs.sidestore.io/)**

## Requirements
To install SideStore, you will need:
- An iPhone, iPad, or iPod touch with a passcode running iOS/iPadOS 15.0 or higher (the iDevice)
- A computer running Windows 8 or higher, macOS High Sierra or higher, or an up-to-date Linux distribution; only for initial install
- An Apple Account (also called an Apple ID)
- A Wi-Fi connection
- Developer Mode (iOS/iPadOS 16+)
> To enable Developer Mode, go to Privacy & Security and scroll down to Developer Mode. Enable it; your phone will restart.

## Preparation
1. On your iDevice, go to the App Store and search "LocalDevVPN".
2. Install the app and open it.
> If you cannot use the App Store as you are in the EU, use [https://api.altstore.io/source/adp.se2crid.me?app=com.jkcoxson.LocalDevVPN](https://api.altstore.io/source/adp.se2crid.me?app=com.jkcoxson.LocalDevVPN) instead.
3. Click Skip and click Connect.
4. Click Allow and enter your password.

### MacOS
5. Go to this link: [https://github.com/nab138/iloader/releases/latest/download/iloader-darwin-universal.dmg](https://github.com/nab138/iloader/releases/latest/download/iloader-darwin-universal.dmg) and download the file.
6. Open the DMG and drag iloader into Applications.

### Windows
> Note: This will only work for 64-bit versions of Windows. Windows 10 on ARM is not supported either.

> To check if your computer is unsupported, open the Run dialog (Win+R) and enter:
> control /name microsoft.system 

> The Control Panel will open. Under the "System" tab, locate "System Type". If you have a "32-bit" operating system, or if you have an "ARM64" processor AND you are using Windows 10, your version of Windows is not supported.
5. Download and install iTunes from the Microsoft Store ([https://apps.microsoft.com/store/detail/9PB2MZ1ZMB1S](https://apps.microsoft.com/store/detail/9PB2MZ1ZMB1S)) or directly from Apple ([https://www.apple.com/itunes/download/win64](https://www.apple.com/itunes/download/win64)).
6. Download the iloader installer as an MSI ([https://github.com/nab138/iloader/releases/latest/download/iloader-windows-x64.msi](https://github.com/nab138/iloader/releases/latest/download/iloader-windows-x64.msi); recommended) or as an EXE ([https://github.com/nab138/iloader/releases/latest/download/iloader-windows-x64.exe](https://github.com/nab138/iloader/releases/latest/download/iloader-windows-x64.exe)).
7. Run the installer.

### Linux
> [https://docs.sidestore.io/docs/installation/prerequisites](https://docs.sidestore.io/docs/installation/prerequisites)

### ChromeOS
> This will likely not work if you have an enrolled Chromebook, as Linux development environment tends to be force-disabled. Depending on how old your Chromebook is, you may not see an option to enable Linux development environment.
5. Go to Settings.
6. Press "About ChromeOS".
7. Scroll down to Developers, then press "Set up" next to Linux development environment.
8. Press Next, then press Install (after setting Disk size).
9. Wait until it finishes.
10. A Terminal window should open. Run `sudo apt-get update && sudo apt-get dist-upgrade`
> If prompted to continue, type 'y'.
11. Once the packages are updated, run `sudo apt-get install usbmuxd fuse curl`
12. Run `uname -m` in order to decide which iloader version to download.
> If x86_64 is outputted, run `curl -fsSLO https://github.com/nab138/iloader/releases/latest/download/iloader-linux-amd64.AppImage` <br>
> If aarch64 is outputted, run `curl -fsSLO https://github.com/nab138/iloader/releases/latest/download/iloader-linux-aarch64.AppImage`
13. Run the following command to ensure usbmuxd has started: `sudo systemctl restart usbmuxd`.
14. In Settings, find Linux developer environment and press it. After that, press Manage USB devices.
15.  Connect your iDevice to your computer using a USB cable. As soon as you see your iDevice, quickly enable it from the list. If you are prompted on your iDevice, trust the computer and enter your passcode.
16.  Run `lsusb` in Terminal and make sure your iDevice is listed. If not, unplug it from your Chromebook and try the previous step again. You should see an output like this when running `lsusb`:
``Bus 001 Device 001: ID 1d6b:0002 Linux Foundation 2.0 root hub
Bus 001 Device 002: ID 05ac:12a8 Apple, Inc. iPhone 5/5C/5S/6/SE/7/8/X/XR
Bus 002 Device 001: ID 1d6b:0003 Linux Foundation 3.0 root hub``
17. In Terminal, run this command to allow iloader to be executable, and to launch iloader. In Step 12, if it outputted x86_64, run the 1st chmod command. If it outputted aarch64, run the 2nd chmod command.
`chmod +x ./iloader-linux-amd64.AppImage
./iloader-linux-amd64.AppImage`
`chmod +x ./iloader-linux-aarch64.AppImage
./iloader-linux-aarch64.AppImage`
> If nothing happens, run `./iloader-linux-amd64.AppImage` or `./iloader-linux-aarch64.AppImage` <br>
> (iloader:1703): dbind-WARNING : 17:45:41.504: AT-SPI: Error retrieving accessibility bus address: org.freedesktop.DBus.Error.ServiceUnknown: The name org.a11y.Bus was not provided by any .service filescCouldn't open libGLESv2.so.2: libGLESv2.so.2: cannot open shared object file: No such file or directory. Aborted <br>
> To fix this error, run `sudo apt update && sudo apt install -y libgles2` <br>
> --Run `sudo ln -sf /usr/lib/x86_64-linux-gnu/libGLESv2.so.2 /usr/lib/libGLESv2.so.2`-- (NOT NEEDED) <br>
> Now, run the command in step 17 again.
18. If iloader isn't showing your iDevice, you can try manually running usbmuxd by running the following commands in the Terminal in another tab: `sudo systemctl stop usbmuxd` and `sudo usbmuxd -v -f`. You may be prompted on your iDevice.

## Installation
1. Connect your iDevice to your computer using a USB cable.
2. Go to Applications on your computer and open iloader. Click Open when prompted. You may need to trust your computer and enter your password on your iDevice.
3. Enter your Apple Account Email and password; it is case-sensitive! It does not need to be the account associated with the iDevice. Afterwards, click Login and wait until it gives a 2FA popup.
4. On your iDevice, click Allow. Afterwards, enter the code it displays into the box in iloader and click Submit.
5. Select your iDevice in iloader (if you're on chromeOS and you can't, good luck fixing it).
6. Click "SideStore (Stable)" and wait until it finishes installing.
> iLoader lets you install IPAs as you would with Sideloadly or Impactor: Instead of choosing "SideStore (Stable)" in iloader, you can "Import IPA" instead. Select the Delta IPA from [https://deltaexploits.gg](https://deltaexploits.gg). Afterwards, wait for it to Sign and Install. Note that this install lasts only 7 days; you will need to use iloader again afterwards.
7. On your iDevice, go to Settings > General > VPN & Device Management. Click the Developer App that shows with your Apple Account email.
8. Trust it and click Allow. For later iOS/iPadOS, it will show as Allow & Restart. Enter your password if you are prompted.
9. Go to your home screen and open SideStore. Click Allow for the local network popup.
10. Click Settings and click "Sign in with Apple Account". Enter your Apple Account email and password; the same one you used for iloader! Afterwards, click Sign in and wait.
11. Click "Got It", then go to My Apps.
12. Click the "7 DAYS" counter next to SideStore. If you receive a prompt asking to revoke or create a new signing certificate, tap 'Yes' or 'Refresh Now'.
> 7 represents the number of days until an app's expiry. It will update dynamically to show the number of days left. Tapping it refreshes the app.
13. Go to [https://deltaexploits.gg](https://deltaexploits.gg) and download the IPA.
> Due to a Delta update, you will need to sign the IPA with any certificate before continuing. You can use IPASignX to do this (read my tutorial about it). <br />
> However, instead of clicking "Install Now", click "Download IPA". Afterwards, do the following: <br />
>> 1. Go to Files and find the signed IPA (Browse > Downloads). Hold it, then tap Rename.
>> 2. Add ".zip" after .ipa (e.g. NAME.ipa > NAME.ipa.zip). Tap "done", then tap "Use .zip".
>> 3. Tap the file again, and hold the Payload folder once it is created.
>> 4. Tap Compress, then hold Payload.zip once it gets created.
>> 5. Tap Rename, then rename the file to Payload.ipa. Tap "done", then tap "Use .ipa". <br />
14. In the My Apps section of SideStore, click the plus (+) button at the top left. Find the Delta IPA you signed with the certificate and click it.
15. Wait until Delta appears. Click Keep App Extensions.
16. Check your Home Screen; you now have Delta!
> ⚠️ DO NOT TURN OFF LOCALDEVVPN OR BACKGROUND REFRESHING WILL NOT WORK (SO YOU WILL HAVE TO SIGN SIDESTORE AGAIN). LocalDevVPN is required to be turned on any time you wish to install, update, or refresh apps in SideStore. <br />
> ⚠️ Updating or resetting your device may invalidate the pairing file, requiring replacement using [this guide](https://docs.sidestore.io/docs/advanced/pairing-file). This may also occur unpredictably due to Apple software behaviour.
