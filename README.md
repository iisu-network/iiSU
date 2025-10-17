# 🚀 Quick Start Guide for iiSU DS

## 1. Before You Begin
iiSU DS is currently in an **early Alpha stage**, focused on building the technical foundation of the launcher for future iterations.  
For now, it is recommended to set it as your **home screen only in controlled test scenarios**.

---

## 2. Preparing Your Asset Library

### 2.1. Paths and Folder Structure
- **ROMs:** Place custom icons inside `iiSULauncher/assets/roms` in any external media directory created by Android for the app (e.g.,  
  `/storage/emulated/0/Android/media/com.iisulauncher/iiSULauncher/assets/roms`).  
  The application will create these folders if they don’t exist.  

- **APPs:** Place custom icons inside `iiSULauncher/assets/android` in any external media directory created by Android for the app (e.g.,  
  `/storage/emulated/0/Android/media/com.iisulauncher/iiSULauncher/assets/android`).  
  The application will create these folders if they don’t exist.  

- **Platforms:** Icons and backgrounds for each system are stored in `iiSULauncher/assets/platforms`, accessible from both `externalMediaDirs` and the legacy path:  
  `/storage/emulated/0/Android/media/com.iisulauncher/iiSULauncher/assets/platforms`.

### 2.2. Recommended Naming Convention
- Use **PNG or JPG** files. For each ROM or App, name the icon as `<sanitized_name>_X.png` (or `.jpg`), where **X** is:
  - `_icon` → Icon displayed on the main screen  
  - `_slide_Y` → Images for the gallery, where **Y** is the index (1, 2, 3 …)  
  - `_hero_Y` → Background images for the top screen, where **Y** is the index (1, 2, 3 …)  

- Names are **automatically sanitized**:
  - Accents and special characters removed  
  - Spaces replaced with underscores  
  - Converted to lowercase  
  - Example: `The Legend: GB` → `the_legend_gb`  

- For platforms you can provide:
  - **Icon:** `<platform>.png`  
  - **List background:** `<platform>_list.png`  
  - **Selected list background:** `<platform>_list_selected.png`  

💡 *Note: The repo includes a `iiSULauncher` folder containing the minimum required assets for configuration.*

---

## 3. First Launch and Shortcuts
In the **Home** section you’ll find the quick-access grid.  
Tap the **“Edit”** button to enable edit mode.  

To pin an app or ROM:
- Open its settings card  
- Hold the icon to enter edit mode, then hold it again to open per APP/ROM Settings  
  - Or with a controller: press **“Y”** to enter edit mode, then **“Start”**  
- Enable the **Shortcut** checkbox in the preferences panel  

This preference is saved **persistently** in the launcher’s configuration.

---

## 4. Choosing Where to Launch Each App or ROM
When launching an app or ROM for the first time, a dialog will appear asking you to choose a screen (**internal or external**) and whether to **remember your selection**.  

If you check the box, the launcher will automatically save this preference for future launches.  

You can also adjust this behavior at any time from the item’s settings dialog:
- **Internal**  
- **External**  
- **Always Ask**  

Here you can also manage shortcuts and app linking.

---

## 5. Organizing the Apps, Games, and Emulators Tabs
The three main tabs (**APPS, GAMES, EMULATORS**).  

To customize:
- Enter edit mode (long-press an app in the corresponding tab)  
- Use the **visibility toggle** to hide items you don’t want  

Visibility is saved **per tab**, so each view keeps its own selection.

---

### 6. Supported Emulators

These cores in Retroarch are supported with custom per-ROM launch commands, layout behavior, and some with artwork mapping (as of the latest build):

- 3do,amiga,arcade,atari2600,atari5200,atari7800,atari800,atarijaguar,atarilynx,atomiswave,c64,channelf,colecovision,cps1,cps2,cps3,dreamcast,famicom,fba,fbneo,gameandwatch,gamegear,gba,gbc,genesis,gw,intellivision,mame,mastersystem,megadrive,msx,msx2,naomi,nds,neogeo,neogeocd,nes,nintendo64,nintendobs,odyssey2,openbor,pcengine,pcenginecd,pce,ps1,ps2,psp,saturn,sega32x,segacd,segamastersystem,sega_md,sega_saturn,sg1000,snes,supergrafx,tg16,tgcd,uzebox,vectrex,virtualboy,wii,wonderswan,wonderswancolor,x68000,xbox,zxspectrum

Other cores and emulator definitions will be added in future versions.

---

### 7. RetroAchievements Integration

iiSU Launcher now supports [RetroAchievements](https://retroachievements.org)!

To enable it, you'll need your **RetroAchievements username** and **Web API Key**.

#### 🔑 How to get your Web API Key:
1. Log into [RetroAchievements.org](https://retroachievements.org).
2. Go to your profile settings.
3. Scroll down to the **Web API Key** section and copy it.

Once you've configured your credentials in iiSU DS, the following will happen:
- In the RetroAchievements tab, you’ll see a summary of your recent activity, showing the most recent games where you’ve unlocked achievements, along with your total points and progress.
- When entering a platform, the launcher will **start hashing your ROMs in the background** to identify them with RetroAchievements.
- While hashing, a loading icon will appear in the top-left corner of each ROM.
- Once a ROM is identified, hovering over it will **trigger a background request** to fetch the list of achievements for that specific game.
  - During this process, you’ll see a loading icon again on that ROM.
  - Once complete, if the ROM doesn’t have a custom icon, it will show the `ImageBoxArt.png` provided by RetroAchievements.

You can view the available achievements at any time by pressing **X** or **Y** on your controller (depending on your button layout).

⚠️ For best performance, avoid requesting achievements for too many games at once. Achievement fetching is currently manual and per-ROM, but **batch fetching and automation will be added soon.**

---

## 8. Project Status
Remember: **iiSU DS is a prototype** aimed at testing on dual-screen and single screen hardware.  
Please use it as a **testbed**, report bugs, and share feedback or features you’d like to see before considering it ready for daily use.

- Thanks to the communities of AYANEO, Retroid, OneXPlayer, and everyone contributing feedback through Discord and Patreon.