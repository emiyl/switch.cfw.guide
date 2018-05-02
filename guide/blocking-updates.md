---
title: Blocking Updates
layout: single
sidebar:
  nav: "side"
---

More experienced users on 2.3.0 and below may launch the Homebrew Launcher via using PegaSwitch [here](/more/homebrew-launcher-(pegaswitch)).
{: .notice--info}

These DNS settings must be set on every network you connect to.
{: .notice--info}

You must have connected to the Nintendo Online Services at least once before proceeding.
{: .notice--info}

After 27th April 2018, the `173.255.238.217` and `45.79.103.52` update blocking DNS servers will not work. Please remove these and replace these with the new ones detailed in the guide to continue blocking updates.
{: .notice--danger}

This will stop your Switch from downloading any future updates. Updates could patch future exploits, leaving you without access to homebrew in the future.

1. Go to the System Settings application
2. Scroll down the menu on the left-hand side and select “Internet”
3. Select “Internet Settings”
4. Select your network
5. Scroll down to “DNS Settings”
6. Set your DNS Settings to “Manual”
7. Change your Primary DNS to `104.236.106.125`
8. Change your Secondary DNS to `62.210.147.20`

## Deleting Downloaded Updates

1. Hold down the "Power" Button
2. Select "Reboot"
3. If that doesn't work, reboot again but hold down **Volume +** and **Volume -** while rebooting
	- Make sure to not select any options in Recovery Mode, only reboot
