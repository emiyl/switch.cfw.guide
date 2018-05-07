---
title: Homebrew Launcher (PegaSwitch)
layout: single
---

While this guide _should_ work, it has not been tested
{: .notice--info}

After 27th April 2018, the `173.255.238.217` and `45.79.103.52` update blocking DNS servers will not work. Please remove these and replace these with the new ones detailed in the guide to continue blocking updates.
{: .notice--danger}

This guide will allow you to install the Homebrew Launcher on 2.0.0 to 2.3.0, using PegaSwitch. This will have to be reinstalled upon each reboot, but will remain active until then.

The Homebrew Launcher allows you to run unsigned, user-made software on your Nintendo Switch on versions 3.0.0 and below. If you would like to run homebrew on version 3.0.0, follow [this guide](/guide/homebrew-launcher).

Make sure to only download homebrew from trusted sources. Running untrusted homebrew could potentially damage your Switch and void your warranty.

If you'd like to read more on the Homebrew Launcher, go to the offical website [here](https://switchbrew.github.io/nx-hbl/){:target="_blank"}.

## Downloads
- The latest version of [PegaSwitch](https://github.com/reswitched/pegaswitch/archive/master.zip)
- The latest version of [node.js](https://nodejs.org/en/){:target="_blank"}
- The latest release of [nx-hbmenu](https://github.com/switchbrew/nx-hbmenu/releases/latest/){:target="_blank"}
- [loader.nsp](/assets/files/loader.nsp)

## Preparations
1. Insert your microSD card into your computer
2. Copy `loader.nsp` to the root of your microSD card
3. Extract the contents of the nx-hbmenu `.zip` file to the root of your microSD card
4. Create a folder called `switch` on the root of your microSD card if it doesn't already exist

## Configuring PegaSwitch
1. Extract the PegaSwitch `.zip` file to a folder on your Desktop
2. Copy `hbmenu.js` to the `usefulscripts` folder in your PegaSwitch folder
3. Install node.js if you haven't already
4. Navigate to the PegaSwitch folder and open your terminal/cmd
5. Run `npm install` to install PegaSwitch
6. Run `node start.js` to start PegaSwitch
  - You may need to use `sudo` on Linux/macOS
7. Write down the IP address displayed on-screen
  - This is usually in the format of `192.168.1.XXX`

## Configuring DNS
1. Launch the System Settings application
2. Scroll down the menu on the left-hand side and select "Internet"
3. Select "Internet Settings"
4. Select your network
5. Scroll down to "DNS Settings"
6. Set your DNS Settings to "Manual"
7. Set your "Primary DNS" and "Secondary DNS" to the IP Address you got earlier from PegaSwitch
8. Save your network settings

## Installation
1. If it was successful, you will see the message, "Registration is required to use this network"
2. Select "Next"
  - The PegaSwitch website should load
  - PegaSwitch on your computer should show that your device is connected
3. Run `evalfile usefulscripts/installFakeNews.js` in your terminal/cmd
4. Reboot your device
  - You should see a PegaSwitch news entry
5. Exit PegaSwitch by pressing `Ctrl+C` twice
6. Run the command `node start.js --webapplet`
7. Select the PegaSwitch news entry on your device
8. Tap to open the "Video"

## Installing Homebrew Applications

1. Make a new directory on the root of your Switch's MicroSD Card called `switch/`
2. Download a homebrew application of your choice from [switchbrew](http://switchbrew.org/index.php?title=Homebrew_Applications){:target="_blank"}, [r/SwitchHacks](https://www.reddit.com/r/SwitchHacks/){:target="_blank"} or [GBAtemp](https://gbatemp.net/forums/285/){:target="_blank"}
3. Extract an archive file if it comes with one
4. Find the `.nro` file and place it into the `switch/` directory on your MicroSD Card
