# Quick Start Guide for iiSU

## 1. Before You Begin
iiSU is currently in an **early Alpha stage**, focused on building the technical foundation of the launcher for future iterations.  
For now, it is recommended to set it as your **home screen only in controlled test scenarios**.

---

## 2. Preparing Your Asset Library

### 2.1. Paths and Folder Structure
- **ROMs:** Place custom icons inside `iiSULauncher/assets/media/roms/consoles/<console_name>/<rom_name>/` in any external media directory created by Android for the app (e.g.,  
  `/storage/emulated/0/Android/media/com.iisulauncher/iiSULauncher/assets/media/roms/consoles/<console_name>/<rom_name>/`).  
  The application will create these folders if they don’t exist.  

- **APPs:** Place custom icons inside `iiSULauncher/assets/media/android/apps/<app_package>/` in any external media directory created by Android for the app:  
  `/storage/emulated/0/Android/media/com.iisulauncher/iiSULauncher/assets/media/android/apps/<app_package>/`.  
  The application will create these folders if they don’t exist.  

- **Platforms:** Icons and backgrounds for each system are stored in `iiSULauncher/assets/platforms`, in any external media directory created by Android for the app:
  `/storage/emulated/0/Android/media/com.iisulauncher/iiSULauncher/assets/platforms`.

- **Themes:** Backgrounds and video backgrounds for themes (each folder inside Themes is a theme) are stored in: 
  `/storage/emulated/0/Android/media/com.iisulauncher/iiSULauncher/assets/Themes/`.

### 2.2. Recommended Naming Convention
- Use **PNG or JPG** files. For each ROM or App, name the icon as:
  - `icon` → Icon displayed on the main screen.
  - `slide_Y` → Images for the gallery, where **Y** is the index (1, 2, 3 …).
  - `hero_Y` → Background images for the top screen, where **Y** is the index (1, 2, 3 …).
  - `title` → Title image for the top screen.

- For platforms you can provide:
  - **Icon:** `<platform>.png`
  - **Title:** `<platform>_title.png`  
  - **List background:** `<platform>_list.png`  
  - **Selected list background:** `<platform>_list_selected.png`  

- For themes you can provide (in a folder inside Themes):
  - **Detail Screen background:** `detail_background.png`/`detail_background_dark.png`
  - **Navigation Screen background:** `home_background.png`/`home_background_dark.png`
  - **Animated Detail Screen background:** `detail_background.mp4`/`detail_background_dark.mp4`
  - **Animated Navigation Screen background:** `home_background.mp4`/`home_background_dark.mp4` 

---

## 3. First Launch and Shortcuts
In the welcome screen, you will be guided through the iiSU setup. If you had a previous version, it is strongly advised to install this new one (just back up your image data beforehand).

In the **Home** section you’ll find the quick-access grid.  
To pin an app or ROM:
- Go to the app or ROM you want to pin
If you are using controlls
- When the App/ROM is on focus press "Start" and chose "Add to HomePage"
If you are touch screen
- Hold the icon, then go back and chose "Add to HomePage"

This preference is saved **persistently** in the launcher’s configuration.

---

## 4. Choosing Where to Launch Each App or ROM
When launching an app or ROM for the first time, a dialog will appear asking you to choose a screen (**this screen or the other screen**) and whether to **remember your selection**.  

In the apps setting you can also manage shortcuts and app linking.

---

## 5. Organizing the Apps, Games, and Emulators Tabs
The three main tabs (**APPS, GAMES, EMULATORS**).  

To customize:
- Enter edit mode (long-press an app in the corresponding tab) or choose the option "Enable edit mode"
- Use the **visibility toggle** to hide items you don’t want  

Visibility is saved **per tab**, so each view keeps its own selection.

---

### 6. Supported Emulators

We support almost all emulators!, if you find an emulator that is not working, please fill a bug and we will fix it!

---

### 7. RetroAchievements Integration

iiSU supports [RetroAchievements](https://retroachievements.org)!

To enable it, you'll need your **RetroAchievements username** and **Web API Key**.

#### How to get your Web API Key:
1. Log into [RetroAchievements.org](https://retroachievements.org).
2. Go to your profile settings.
3. Scroll down to the **Web API Key** section and copy it.

Once you've configured your credentials in iiSU, the following will happen:
- In the RetroAchievements tab, you’ll see a summary of your recent activity, showing the most recent games where you’ve unlocked achievements, along with your total points and progress.
- In each platform, you can choose to **start hashing your ROMs** and also fech data from RA to identify them with RetroAchievements.
- While hashing, a loading icon will appear in the top-left corner of each ROM.
- Once a ROM is identified, hovering over it will **trigger a background request** to fetch the list of achievements for that specific game.
  - During this process, you’ll see a loading icon again on that ROM.
  - Once complete, if the ROM doesn’t have a custom icon, it will show the `ImageBoxArt.png` provided by RetroAchievements.

You can view the available achievements at any time by pressing **X** or **Y** on your controller (depending on your button layout).

For best performance, avoid requesting achievements for too many games at once. Achievement fetching is currently manual, you can preload all in the welcome screen.

### 8. IGDB Integration

iiSU supports [IGDB](https://www.igdb.com/)!

To enable it, you'll need your **Client id** and **Client secret**.

#### How to get your credentials from (https://api-docs.igdb.com/#getting-started):
- Sign Up with [Twitch](https://dev.twitch.tv/login) for a free account
- Ensure you have Two Factor Authentication [enabled](https://www.twitch.tv/settings/security)
- Register your application in the [Twitch Developer Portal](https://dev.twitch.tv/console/apps/create)
- The OAuth Redirect URL field is not used by IGDB. Please add ’localhost’ to continue.
- The Client Type must be set to Confidential to generate Client Secrets, follow this example:
<img width="773" height="531" alt="image" src="https://github.com/user-attachments/assets/690afe68-b587-4299-a039-e09553cedbeb" />

- [Manage](https://dev.twitch.tv/console/apps) your newly created application
<img width="1252" height="47" alt="image" src="https://github.com/user-attachments/assets/2186e316-7d24-4dc0-a298-5c9b7bb96acf" />

- Generate a Client Secret by pressing "New Secret"
<img width="758" height="182" alt="image" src="https://github.com/user-attachments/assets/48948944-03d8-4726-a8ec-829eb45a3342" />


- Take note of the Client ID and Client Secret


Once you've configured your credentials in iiSU, the following will happen:

---

## 8. Project Status
Remember: **iiSU** is aimed at testing on dual-screen and single screen hardware.  
Please use it as a **testbed**, report bugs, and share feedback or features you’d like to see before considering it ready for daily use.

- Thanks to the communities of AYANEO, Retroid, OneXPlayer, and everyone contributing feedback through Discord and Patreon.
