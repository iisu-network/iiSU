<p align="center">
  <img 
    src="https://raw.githubusercontent.com/iisu-network/iiSU/a5012c3066d6db158909bdec78b7c655da0d789a/.github/assets/iiSU_Logo.svg"
    alt="iiSU Logo"
    width="60%"
    style="max-width: 300px;"
  />
</p>

<h3 align="center">The visuals-first emulation frontend</h3>

<p align="center">
  <a href="https://github.com/iisu-network/iiSU/releases"><img src="https://img.shields.io/github/v/release/iisu-network/iiSU?label=latest&color=7c3aed" alt="Latest Release"/></a>
  <a href="https://discord.com/invite/iisu"><img src="https://img.shields.io/discord/1072873391855501312?label=discord&logo=discord&color=5865F2" alt="Discord"/></a>
  <a href="https://ko-fi.com/iisunetwork"><img src="https://img.shields.io/badge/support-ko--fi-FF5E5B?logo=kofi" alt="Ko-fi"/></a>
</p>

<p align="center">
  <a href="https://discord.gg/iisu">Discord</a> ·
  <a href="https://iisu.network">Website</a> ·
  <a href="https://github.com/iisu-network/iiSU/releases">Download</a> ·
  <a href="https://iisu.network/faq">FAQ</a>
</p>

---

# iiSU
iiSU is an emulation frontend in alpha, being developed Android-first. A frontend effectively replaces your home screen launcher with a UI fit to display and launch your games and apps beautifully.

> [!WARNING]
> iiSU is a **frontend**, not an emulator - it does **not include games or emulators**.

Beyond the app itself, the iiSU team is working to deliver web services while fueling a community-wide effort to enhance the emulation scene with stylish assets and designs that reach beyond the core app.

## Showcase
<p align="center">
  <img 
    src="https://github.com/iisu-network/iiSU/blob/main/.github/assets/SingleScreen_Demo.png?raw=true"
    alt="iiSU Single Screen Demo"
    height="300"
    style="max-width: 50%;"
  />
  <img 
    src="https://github.com/iisu-network/iiSU/blob/main/.github/assets/DualScreen_Demo.png?raw=true"
    alt="iiSU Dual Screen Demo"
    height="300"
    style="max-width: 50%;"
  />
</p>

## Install & Updates
Download the latest APK from the [Releases page](https://github.com/iisu-network/iiSU/releases).

iiSU includes a built-in updater, but you can also keep it up to date using Obtainium:

<p align="center">
  <a href="http://apps.obtainium.imranr.dev/redirect.html?r=obtainium://app/%7B%22id%22%3A%22com.iisulauncher%22%2C%22url%22%3A%22https%3A%2F%2Fgithub.com%2Fiisu-network%2FiiSU%22%2C%22author%22%3A%22iisu-network%22%2C%22name%22%3A%22iiSU%22%7D">
    <img 
      src="https://raw.githubusercontent.com/ImranR98/Obtainium/refs/heads/main/assets/graphics/badge_obtainium.png"
      alt="Get it on Obtainium"
      height="55"
    />
  </a>
</p>

---

## Quick Start Guide

### 1. Before You Begin
iiSU is currently in an **early Alpha stage**, focused on building the technical foundation of the launcher for future iterations.  
Bugs and issues will exist, please report them to the team at https://github.com/iisu-network/iiSU/issues
This guide covers the essentials to get iiSU up and running quickly.  
For help, issues, or questions, join our [Discord](https://discord.com/invite/iisu).

---

### 2. First Launch and Shortcuts
On your first launch of iiSU, you'll be welcomed with the **interactive onboarding**. This is where you'll be prompted to choose your main settings, configs and home menu shortcuts for iiSU. It's also where you'll be able to optionally **generate retroachievement hashes**, do an **initial library scrape**, **link ES-DE Metadata**, and **pre-cache** your library.

> [!TIP]
> You can skip any of these, and do any of these actions at any time from iiSU. Onboarding just gives you an easy flow to get you setup quickly.
> You can also **relaunch onboarding** at any time

Below is a brief overview of each step of onboarding

1) Welcome - This page is a welcome page, welcoming you to iiSU
2) Dual Screens - If an external display is detected, this page allows you to choose which screen displays what media. You can swap screens at any time by pressing Y.
3) Customization - In this page, you can choose your default theming colour, browsing style, and a selection of key settings, to get iiSU looking exactly as you'd like it to look, as soon as you launch.
4) ROM Import - On this page, you can select your ROM folder, and link ES-DE metadata if you're changing frontends. You can also change your iiSU media storage location and check the detected systems. If you have a RomM server, you can link your server here as well. RomM support is currently an **experimental** feature.
5) Quick Access Apps - This page allows you to choose apps to add to the home page. Apps can be added/removed later!
6) RetroAchievements Login - If you would like to sync your RetroAchievements, you can connect to your account here. To get your API key, go to https://retroachievements.org/settings and scroll down.
7) Services - Here you can optionally input keys and sign in data for a host of scraping services to be used in the app
8) Asset Prep - This page indexes your library and prepares your media.
9) RetroAchievement Data - In order to show RetroAchievement data, you need to hash your roms. This page allows you to easily hash them!
10) Scrape Pass - If you would like to perform an initial scrape, you can do this. This isn't required if you have linked your ES-DE Metadata or would not like to scrape just yet
11) Overview - This page shows a brief overview of what's been setup!

---

#### 3. Post-Onboarding:
Once onboarding is complete, there are a few recommended (but not required) tasks you can do.
 - Update everything
    - Open Settings (select), go to iiSU Settings -> Updates, and check for updates.
    - The key ones to check are for Starter Pack Updates, emuladores, and iiSU updates.
    - If an update is found, simply install and apply the update!
 - Swap A/B X/Y
    - If you want to use a Nintendo-Style layout, head to Settings (select), then iiSU Settings -> Input -> "Swap A/B and X/Y Buttons"
 - Enable/Disable Dark Mode Icons
    - To toggle these, head to Settings (select), then iiSU Settings -> Appearance -> Theme Media -> "Use Dark Mode Platform Icons"
 - Check Console Emulators
    - If a console isn't launching, check to make sure it is set to use the correct emulator.
    - You can do this by opening Quick Settings (select) whilst the console is selected, heading to "Console Settings", "Edit Console Settings" and selecting the correct emulator.
      - One common issue is RetroArch games not launching, please make sure the correct RetroArch version is selected for your device.
    - Make sure to Update the console in the summary tab once you've done!

> [!TIP]
> You can set iiSU to replace your device's home screen!
> Just open Settings, search for "Default Home App" and select iiSU

---

#### 4. Home Menu & Collections

To add items to the home menu, simply select it, open Quick Settings with select, and press "Add to home page".

From the home menu, you're also able to make collections. To add a ROM to a collection, select the game, press select and press "Add to Collection".

---

#### 5. Supported Emulators

We support almost all emulators on Android! If you find an emulator that is not working, please fill out a github issue and we will fix it as soon as we can.

---

#### 6. RetroAchievements Integration

iiSU supports [RetroAchievements](https://retroachievements.org)!

To enable it, you'll need your **RetroAchievements username** and **Web API Key**.

##### How to get your Web API Key:
1. Log into [RetroAchievements.org](https://retroachievements.org).
2. Go to your profile settings.
3. Scroll down to the **Web API Key** section and copy it.

Once you've configured your credentials in iiSU, the following will happen:
- In the RetroAchievements tab, you’ll see a summary of your recent activity, showing the most recent games where you’ve unlocked achievements, along with your total points and progress.
- In each platform, you can choose to **start hashing your ROMs** and also fetch data from RA to identify them with RetroAchievements.
- While hashing, a loading icon will appear in the top-left corner of each ROM.
- Once a ROM is identified, hovering over it will **trigger a background request** to fetch the list of achievements for that specific game.
  - During this process, you’ll see a loading icon again on that ROM.
  - Once complete, if the ROM doesn’t have a custom icon, it will show the `ImageBoxArt.png` provided by RetroAchievements.

You can view the available achievements at any time by pressing **X** or **Y** on your controller (depending on your button layout).

---
> [!IMPORTANT]
> iiSU is still in Alpha, however it is approaching a Beta release.
> Bugs can be expected, there's a lot of work behind the scenes making sure it works as smoothly as possible!
> A huge thank you to the communities of AYN, Anbernic, AYANEO, Retroid, OneXPlayer, and everyone contributing feedback through Discord and Patreon, and the supporters on KoFi. It really goes a long way to motivate the team and help develop and create our shared vision!
