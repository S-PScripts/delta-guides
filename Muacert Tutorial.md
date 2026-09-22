# Muacert - Tutorial

## Installing the anti-revoke DNS
1. Turn off any VPNs you may have enabled.
2. If you haven't installed the anti-revoke DNS yet, copy this link and paste it into Safari: https://github.com/dns-khoindvn/oci-auto-vm/releases/download/DNS/khoindvn.mobileconfig.
3. Press Open, then open the Settings app on your phone.
4. Go to General, then press VPN and Device Management.
5. Press on khoindvn.io.vn, and install the DNS.
6. Turn off other DNSes you may have on. 
   
## Topping up
> If Muacert doesn't load, turn your Wi-Fi off and use mobile data. You may need to use a VPN (preferably ZIC VPN).
1. Navigate to https://muacert.com/topup (use Safari).
2. Click on the Apple Pay / Google Pay / Credit Card option, then select "Understood, go to BuyMeACoffee" on the confirmation prompt.
3. Enter your desired top-up amount (preferably at least **$4 USD**)
> While Muacert lists the input in USD, the platform automatically adjusts for local currency conversions. For example, if you are purchasing from the UK and enter "4" in the BuyMeACoffee box, your account will actually be credited $5.34 USD due to the exchange rate.

> For other methods of purchase, join the Ksign Support server: https://discord.gg/twjKH5qxFZ
4. Once you purchase, your account should get topped up.

## Purchasing a certificate
1. Go to https://muacert.com/add.
2. Press on the "GET UDID" button.
3. Press on Open.
4. Go to the Settings app on your phone, then go to General -> VPN and Device Management.
5. Install the muacert configuration profile, which will provide the UDID.
> If Muacert does not work, use https://udid.tech/ and enter the UDID given manually into the "Enter UDID" box.
6. Select one of the certificate  options available, provided it is not above your balance.
7. Confirm your UDID is correct, and then Add Device.
8. Your balance will be deducted, and your phone will (hopefully) be able to install from Muacert now.
> To check if your device was added successfully, go to https://muacert.com/dashboard and check the list of REGISTERED DEVICES.

## Signing 
1. Go to https://muacert.com/sign.
2. Choose Ksign or Esign 2.0, preferably, then press Sign and Download App.
3. If nothing installs, turn your Wi-Fi off and use mobile data. You may need to use a VPN (preferably ZIC VPN) (turn VPN off afterwards)

## Trusting the application
1. Enable Developer Mode by going to Settings -> Privacy & Security, and scrolling to the bottom.
2. Restart your phone, and you should be able to open the application you installed.
3. Read https://github.com/S-PScripts/delta-guides/blob/main/Using%20KSign%20(IPA).md

## Downloading certificate (only needed for old Esign)
1. Go to https://muacert.com/dashboard.
2. Scroll down to REGISTERED DEVICES.
3. Press on your device, then press "Download certificate zip file".
4. Open Esign, then press the ... button at the top right.
5. Import the certificate ZIP, then press it and unzip it.
6. Open the certificate folder, press the .mobileprovision file, and import it.
7. Press the .p12 file, and import it after entering the password ("1").

<img width="325" height="615" alt="image" src="https://github.com/user-attachments/assets/ec3a47e0-3e92-4fa7-9dbc-16ae14f5c0d4" />
