---
title: Homebrew Launcher
layout: single
---

The DNS settings must be set on every network you connect to.
{: .notice--info}

After 27th April 2018, the `173.255.238.217` and `45.79.103.52` update blocking DNS servers will not work. Please remove these and replace these with the new ones detailed in the guide to continue blocking updates.
{: .notice--danger}

This guide will allow you to install the Homebrew Launcher on version 3.0.0, using the ReSwitched DNS. This will have to be reinstalled upon each reboot, but will remain active until then.

The Homebrew Launcher allows you to run unsigned, user-made software on your Nintendo Switch on versions 3.0.0 and below. If you would like to run homebrew on versions 2.0.0 to 2.3.0, follow [this guide](/guide/homebrew-launcher-(pegaswitch)).

Make sure to only download homebrew from trusted sources. Running untrusted homebrew could potentially damage your Switch and void your warranty.

If you'd like to read more on the Homebrew Launcher, go to the offical website [here](https://switchbrew.github.io/nx-hbl/){:target="_blank"}.

Update blocking will not be necessary after this step, as the Homebrew Launcher DNS automatically blocks updates for you.

## Downloads

- The latest version of [nx-hbmenu](https://github.com/switchbrew/nx-hbmenu/releases/latest){:target="_blank"}

## Instructions

2. Remove your MicroSD Card from your Nintendo Switch and insert your it into your computer
3. Extract the nx-hbmenu `.zip` file
4. Place hbmenu.nro onto the root of your MicroSD Card
5. Eject your MicroSD Card from your computer and put it back in your Nintendo Switch
6. Launch the System Settings application
7. Scroll down the menu on the left-hand side and select "Internet"
8. Select "Internet Settings"
9. Select your network
10. Scroll down to "DNS Settings"
11. Set your DNS Settings to "Manual"
12. Set your "Primary DNS" to `104.236.106.125`
12. Set your "Secondary DNS" to `62.210.147.20`
13. Perform a connection test
  - If this is successful, a pop-up will tell you that "Registration is required to use this network."
14. Click Next
14. When the Homebrew Launcher page loads, click "Install"
  - If you see "2000-1337" on your screen, the Homebrew Launcher installation has succeeded.
  - If you do not, reboot and perform a connection test again
15. Reboot the device
16. Go to the System Settings application
17. Scroll down the menu on the left-hand side and select "Internet"
18. Select "Test Connection"
  - If this is successful, a pop-up will tell you that "Registration is required to use this network."
19. Click "Run"
20. Exit when prompted
21. Go to the Home Menu
22. Click the Album icon

## Install Homebrew Launcher via eShop

You must re-run the "Run" section of the exploit after each reboot through a browser applet. There are more convenient ways to launch it than through a Connection Test, such as through the eShop. You won't be using it anyway if you're on 3.0.0, as you'd need to update to use it.

1. Create a second account on your device.
  - Do not connect to a Nintendo account
2. Launch the eShop Applications
3. Select the second account you created
4. Select "Sign In and link"
5. The Homebrew Launcher page will load
6. Select "Run"

## Installing Homebrew Applications

1. Make a new directory on the root of your Switch's MicroSD Card called `switch/`
2. Download a homebrew application of your choice from [switchbrew](http://switchbrew.org/index.php?title=Homebrew_Applications){:target="_blank"}, [r/SwitchHacks](https://www.reddit.com/r/SwitchHacks/){:target="_blank"} or [GBAtemp](https://gbatemp.net/forums/285/){:target="_blank"}
3. Extract an archive file if it comes with one
4. Find the `.nro` file and place it into the `switch/` directory on your MicroSD Card
