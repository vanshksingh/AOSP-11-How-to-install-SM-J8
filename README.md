# AOSP-11 How to install SM-J8
 /*

* Your warranty is no longer valid.(or it isn't ? who am I to judge)

*

* I am not responsible for bricked devices, dead SD cards, broken touchscreens,

* thermonuclear war, or you getting fired because the alarm app failed. Please

* do some research if you have any concerns about features included in this package

* before flashing it! YOU are choosing to make these modifications, and if

* you point the finger at me for messing up your device, I will laugh at you.

*

Full-AOSP11.img or Go-AOSP.img How to install SM-J8 ~vks
DISCLAIMAR: It is a gsi and not a ROM. I am not responsible for anything ,
proceed at your own risk , All files are properties of their respective owner.

Full-AOSP11.img
It is just flashed with playstore and can use any app

Go-AOSP11.img
It is pre-flashed with Go-apps , and cannot install
Google-full nor the assistant

What works (TESTED ON SM-J810G)
-Calls , SMS
-Data (Enable LTE in data setting , default edge)
-Fingerprint
-Both Camera and Flash
-Audio
-Screen Mirroring
-Basically everything

What dosen't work
-No bugs , Everything works , stable too.

IMPORTANT:You will need an android10 stock vendor.

The incuded .zip contains
-Odin3
-Odin Flashable TWRP , By @goldfish07 (Telegram grpoup = https://t.me/galaxyj8 )
-Nik-gapps-pico-arm64-11.zip (Propietary)(yes it is arm64 , and yes it is not gapps)
[Not there in Go-edition]
-Full-AOSP11.img or Go-AOSP.img (Non compressed/zipped iso)[what you chose]
-Device-ID.apk

Unzip the container file , and copy all these to sd card or an otg pendrive(recomended)
, PC MTP Dosent work in recovery.
Procedure.
1. Flash TWRP with ODIN (Lookup for procedure , and install drivers)
2. Boot into Custom Recovery
3. Wipe > Format_Data > Type yes (Swipe to reset dosen't work, data backup-
-would be a good idea)
4.Navigate to your copied files , select Flash image > V, Flash in system.

[Skip steps 5-6 for Go-edition]
5.Go to wipe (after flash), Advanced wipe > System > Repair or change File System >-
-Resize File System (This Prevents Error70 Insufficient Space in Gapps)
6.Flash NikGapps (select Flah from Zip) , If flash shows Error70 , Repeat From Step 3.

7.Reboot Enjoy

IMPORTANT:-

How to Fix the “Device is not Certified by Google” Error

[Your device will still say it is uncertified in the Google Play Store settings.
This is normal. All this fix does is white-list your uncertified device so you
can still use Google apps and services.]

Steps.

Install the Device+ID.apk (Included)

Open the app , Tap the Google Service Framework (GSF)

Copy it

Go to this website-
Sign in - Google Accounts

Sign-in

Paste/Copy GSF code in the box

Complete captcha (sorry dosen't work for robots)

Register (The box goes red , it's totally fine)

Reboot

After a few mins you should be able to sign in

(Don't worry , it will keep saying that not certified but after
a while it will let you sign in, and turn off notification for play
protect to remove annoying notification)

For more info-
www.xda-developers.com
How to Fix the "Device is not Certified by Google" Error
Are you having trouble with signing in to your Google account? Can't access the Google Play Store or use Google apps like Gmail, Maps, Play Music, or Photos? Seeing a "device is not certified by Google" error? Here's how to fix that.
www.xda-developers.com


Fixed:
1.Gapps Flash Error70 No space
2.Device Is not certified error

Notice:
1.Maps keep closing , Though maps-go , waze work fine.(Probably a google issue)
2.Bootanimation cannot be changed (Though if you find the folder you can)
3.Stock-Camera saves photos sideways , use Googlecamera.apk or any other to fix issue.
4.Play Services can be broken
5.Check for new releases on source


@vanshksingh



use latest nikgapps from https://sourceforge.net/projects/nikgapps/files/Releases/NikGapps-R/
to resolve play services bug , and / or other bugs
