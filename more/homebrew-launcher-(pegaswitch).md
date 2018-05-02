---
title: Homebrew Launcher (PegaSwitch)
layout: single
sidebar:
  nav: "side"
---

This guide is aimed towards the experienced in console hacking.
{: .notice--info}

If you have little experience with console hacking, I recommend [blocking updates](/guide/blocking-updates) and waiting for a different method to become available.
{: .notice--danger}

This guide will allow you to install the Homebrew Launcher on 2.3.0 and below, using PegaSwitch.

## Downloads
- [PegaSwitch](https://pegaswitch.com/){:target="_blank"}
- [loader.pfs0](/assets/files/loader.pfs0)
- [nx-hbmenu](https://github.com/switchbrew/nx-hbmenu/releases/latest/){:target="_blank"}

## Instructions
1. Insert your microSD card into your computer
2. Copy `loader.pfs0` to the root of your microSD card
3. Extract the contents of the nx-hbmenu `.zip` file to the root of your microSD card
4. Launch PegaSwitch
5. Save this [JavaScript snippet](/assets/files/hbmenu.js){:target="_blank"} as `hbmenu.js`
6. Run `evalfile hbmenu.js` in PegaSwitch
7. Close your browser and open your gallery app
