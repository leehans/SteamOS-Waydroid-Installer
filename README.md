# SteamOS Android Waydroid Installer

A shell script to easily install / uninstall Android ([via Waydroid](https://waydro.id/)) on the Steam Deck running on SteamOS.

> **NOTE**\
> If you are going to use this script for a video tutorial, PLEASE reference on your video where you got the script! This will make the support process easier!
> And don't forget to give a shoutout to [@10MinuteSteamDeckGamer](https://www.youtube.com/@10MinuteSteamDeckGamer/) / ryanrudolf from the Philippines!
>

<b> If you like my work please show support by subscribing to my [YouTube channel @10MinuteSteamDeckGamer.](https://www.youtube.com/@10MinuteSteamDeckGamer/) </b> <br>
<b> I'm just passionate about Linux, Windows, how stuff works, and playing retro and modern video games on my Steam Deck! </b>
<p align="center">
<a href="https://www.youtube.com/@10MinuteSteamDeckGamer/"> <img src="https://github.com/ryanrudolfoba/SteamOS-Waydroid-Installer/blob/main/10minute.png"/> </a>
</p>

<b>Monetary donations are also encouraged if you find this project helpful. Your donation inspires me to continue research on the Steam Deck! Clover script, 70Hz mod, SteamOS microSD, Secure Boot, etc.</b>

<b>Scan the QR code or click the image below to visit my donation page.</b>

<p align="center">
<a href="https://www.paypal.com/donate/?business=VSMP49KYGADT4&no_recurring=0&item_name=Your+donation+inspires+me+to+continue+research+on+the+Steam+Deck%21%0AClover+script%2C+70Hz+mod%2C+SteamOS+microSD%2C+Secure+Boot%2C+etc.%0A%0A&currency_code=CAD"> <img src="https://github.com/ryanrudolfoba/SteamOS-Waydroid-Installer/blob/main/QRCode.png"/> </a>
</p>

## Disclaimer
1. Do this at your own risk!
2. This is for educational and research purposes only!

## [Video Tutorial - SteamOS Android Waydroid Installer](https://youtu.be/8S1RNSqFDu4?si=oCfwYNbs8u9sMKGr)
[Click the image below for a video tutorial and to see the functionalities of the script!](https://youtu.be/06T-h-jPVx8?si=pTWAlmcYyk9fHa38)
</b>
<p align="center">
<a href="https://youtu.be/06T-h-jPVx8?si=pTWAlmcYyk9fHa38"> <img src="https://github.com/ryanrudolfoba/SteamOS-Waydroid-Installer/blob/main/android.jpg"/> </a>
</p>

## What's New (as of February 02 2024)
1. added cage launcher for multi-touch support
2. rewrite the script - instead of building from source this now installs prebuilt binaries
3. easier and quicker to install
4. added support for SteamOS 3.5.13 Preview

## What's New (as of December 07 2023)
1. this now works with [casualsnek script!](https://github.com/casualsnek/waydroid_script)
2. added libndk arm translation layer (via casualsnek script)
3. added widevine (via casualsnek script). This is needed for Netflix and Disney+
4. waydroid fingerprint identifies as a [Pixel 5 redfin.](https://github.com/Quackdoc/waydroid-scripts) This is needed for Netflix
5. new method for detecting controller [via Saren method](https://gist.github.com/Saren-Arterius/c5bc39199552a5c244449b0ce467d6b6)

## What's New (as of November 26 2023)
1. cleanup and removed support for SteamOS 3.4.x due to SteamOS 3.5.x already went to stable
2. removed PlasmaNested.sh as this is already included in SteamOS 3.5.x
3. removed the bundled weston binary (only useful when on SteamOS 3.4.x)

## What's New (as of November 15 2023)
1. initial release

## Prerequisites for SteamOS
1. sudo password should already be set by the end user. If sudo password is not yet set, the script will ask to set it up.

## NOTE IF YOU ARE USING AN OLDER VERSION OF MY SCRIPT
1. [Uninstall first if you are using an older version.](https://github.com/ryanrudolfoba/SteamOS-Waydroid-Installer/tree/main#i-dont-want-this-anymore-i-want-to-uninstall)

## How to Use
1. Go into Desktop Mode and open a konsole terminal.
2. Clone the github repo. \
   cd ~/ \
   git clone https://github.com/ryanrudolfoba/steamos-waydroid-installer
3. Execute the script! \
   cd ~/steamos-waydroid-installer \
   chmod +x steamos-waydroid-installer.sh \
   ./steamos-waydroid-installer.sh
4. Script will automatically install Waydroid together with the custom config. Install will roughly take around 5mins depending on the internet connection speed.
5. Once done exit the script and go back to Game Mode.

## Launching Waydroid
1. Go to Game Mode.
2. Run the Waydroid launcher.

## I dont want this anymore! I want to uninstall!
1. Go to Desktop Mode.
2. Open konsole terminal and type the commands - \
   cd ~/Android_Waydroid \
   ./uninstall.sh
3. Enter the sudo password when prompted.
4. Waydroid and the custom configs will be uninstalled.

## A Note on SteamOS Updates
When there is a SteamOS update the waydroid will be wiped. This is normal behavior due to how SteamOS applies updates. \
Re-run the script again but if the SteamOS update contains a new kernel version the script will exit immediately. \
Please file an issue report when this happens so I can compile a binder kernel module to match the SteamOS update.

## List of Games Tested with Demo Gameplay
[Plants vs Zombies](https://youtu.be/rnb0z1LtDN8)
