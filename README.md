# 🚀 Quick Start Guide for iiSU DS

## 1. Before You Begin
iiSU DS is currently in an **early Alpha stage**, focused on building the technical foundation of the launcher for future iterations.  
For now, it is recommended to set it as your **home screen only in controlled test scenarios**.

---

## 2. Preparing Your Asset Library

### 2.1. Paths and Folder Structure
- **ROMs:** Place custom icons inside `LairLauncher/assets/roms` in any external media directory created by Android for the app (e.g.,  
  `/storage/emulated/0/Android/media/com.lairlauncher/LairLauncher/assets/roms`).  
  The application will create these folders if they don’t exist.  

- **Platforms:** Icons and backgrounds for each system are stored in `LairLauncher/assets/platforms`, accessible from both `externalMediaDirs` and the legacy path:  
  `Android/media/com.lairlauncher/LairLauncher/assets/platforms`.

### 2.2. Recommended Naming Convention
- Use **PNG or JPG** files. For each ROM, name the icon as `<sanitized_name>_X.png` (or `.jpg`), where **X** is:
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

💡 *Note: The repo includes a `LairLauncher` folder containing the minimum required assets for configuration.*

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
The three main tabs (**APPS, GAMES, EMULATORS**) display all content by default.  

To customize:
- Enter edit mode (long-press an app in the corresponding tab)  
- Use the **visibility toggle** to hide items you don’t want  

Visibility is saved **per tab**, so each view keeps its own selection.

---

## 6. Current Emulator Compatibility
The included configuration currently only defines launches for **RetroArch** on **Game Boy**, using the **Gambatte** and **SameBoy** cores.  

Other cores and emulator definitions will be added in future versions.

---

## 7. Project Status
Remember: **iiSU DS is a prototype** aimed at testing on dual-screen hardware.  
Please use it as a **testbed**, report bugs, and share feedback or features you’d like to see before considering it ready for daily use.
