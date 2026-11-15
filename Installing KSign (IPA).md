# Installing Delta via KSign
Complete step-by-step installation guide for iOS devices

## Preparation Checklist
- Disable VPNs: Turn off any active VPN connections on your iOS device.
- Disable Secondary DNS: Remove or disable any non-standard DNS configurations.
- Remove Old Versions: If you currently have Direct Install Delta installed, delete it completely.

## Install Anti-Revoke DNS
Install the profile below to prevent enterprise certificates from being revoked by Apple:
https://github.com/dns-khoindvn/oci-auto-vm/releases/download/DNS/khoindvn.mobileconfig

### Need to use a VPN to play Delta?
Copy and install this VPN-compatible profile instead:
https://wsfteam.xyz/files/configurationprofiles/madNS-CP144.mobileconfig

1. Paste the copied link into Safari and press Go.
2. Tap Allow when prompted, then tap Close.
3. Open device Settings → General → VPN & Device Management.
4. Tap Khoindvn and select Install (Ignore any security warnings).

## Install KSign App
Try installing the first KSign profile from https://khoindvn.io.vn. If it shows "Open in iTunes", tap Open and then Install.
> If you get an "Integrity cannot be verified" white icon, delete it and try the next certificate on the list. Repeat until one works. Certificates that work vary for every user.

### KSign prompt issues or not installing?
If you see "Open in iTunes" but no install prompt follows (or you do not even get "Open in iTunes):
- Switch from Wi-Fi to Cellular Data (or vice versa).
- Connect to a personal hotspot.
- Last Resort (ZIC VPN): Install ZIC VPN - Safe Surfer from the App Store, set system language to English, connect, then retry KSign installation. Turn off ZIC VPN once installed.

## Trusting KSign Certificate
Once KSign displays an "Untrusted Enterprise Developer" warning on startup, follow these steps:
1. Enable Airplane Mode to prevent instant revocation.
2. Go to Settings → General → VPN & Device Management.
3. Tap the Enterprise App certificate name and select Trust.
4. Restart your iOS device if necessary, then turn Airplane Mode back off.

## Troubleshooting

### Error Definitions
- "Integrity Could Not Be Verified": Certificate blacklisted/revoked. Delete KSign and use a different certificate link.
- "Unable to Verify App / Internet Connection Required": Try deleting and reinstalling the same KSign. If persistent, switch certificates.
- "No Longer Available" or Sudden Crashing: Certificate has expired or been revoked. Delete both KSign and Delta and start over with a fresh certificate.

### All KSign Certificates Revoked / Blacklisted?
If every free certificate fails to install, consider these alternatives:

- Direct Install: Use Direct Install links if currently operational.
- Computer Sideloading: Sideload via PC/Mac using SideStore, Sideloadly, or Impactor.
- BlacklistBeGone: Compatible with computer setups on iOS 17.0 - 18.0.1.
- Paid Certificates: Purchase private certificates via services like MUA Cert or ArcticSign.
