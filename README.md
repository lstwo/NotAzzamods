# lstwoMODS (formerly "NotAzzamods")

A free recreation of Azzamods for Wobbly Life containing a lot of Azzamods mods but also more than double original ones.

You can open the menu in game using F2.

# Installation Requirements

Requires [ShadowLib](https://github.com/lstwo/ShadowLib/releases) and [BepInEx 5.X](https://github.com/BepInEx/BepInEx/releases/tag/v5.4.23.2)

> [!NOTE]
> NotAzzamods only supports BepInEx 5.X for Mono so far

# Compatibility Chart

| **Mod**           | **Wobbly Server Util** | **Wobbly's Fav**       |
| ----------------: | :--------------------: | :--------------------: |
| **Compatibility** | ✅Fully compatible    | 🟨 Most Functions Work |

# Automatic Installation (If available)

If your release has an installer zip, you can install it like this:

1. Download Installer from [the releases page](https://github.com/lstwo/lstwoMODS/releases)
2. Unzip the File
3. Double Click the **EXE File**

> [!NOTE]
> You may have to create an exception for your anti virus to allow this file

If it didn't work try the manual installation:

# Manual Installation

> [!WARNING]
> This Guide is currently broken.
>
> While I'm working on fixing it just:
>
> Download the installer > unzip it > copy all files of the `files` folder > paste them into your wobbly life folder

## Step 1: Install BepInEx 5
1. Download **BepInEx 5** (Mono version) for Windows x64 from the official [BepInEx GitHub releases](https://github.com/BepInEx/BepInEx/releases) (The file should be called something along the lines of `BepInEx_win_x64_5.x.x.x.zip`).
2. Copy & Paste the contents of the downloaded zip file into your Wobbly Life game folder.
   - The folder should look like this after extraction:
     ```
     Wobbly Life
     ├── BepInEx
     |   ├── core
     |   └── ...
     ├── Mod Tools
     ├── MonoBleedingEdge
     ├── Wobbly Life_Data
     ├── changelog.txt
     ├── doorstop_config.ini
     ├── opengl32.log
     ├── steam_appid.txt
     ├── UnityCrashHandler64.exe
     ├── UnityPlayer.dll
     ├── version.txt
     ├── winhttp.dll
     └── Wobbly Life.exe
     ```

## Step 2: Download lstwoMODS
1. Go to [lstwoMODS Releases](https://github.com/lstwo/lstwoMODS/releases) and download the latest version's files:
   - `lstwoMODS.dll` (in older versions this might be named `NotAzzamods.dll`)
   - `CustomItems.dll` (may not exist in older versions but required for future updates)

## Step 3: Download Required Dependencies
Download **ShadowLib** from its release page. You need these files:
   - `ShadowLib.dll`
   - `lstwo.shadowlib`
   - `UniverseLib.Mono.dll`

## Step 4: Install Plugins
1. Navigate to the `BepInEx/plugins` folder inside your Wobbly Life game folder.
2. Copy the following files into the `plugins` folder:
   - From `lstwoMODS`:
     - `lstwoMODS.dll` (or `NotAzzamods.dll` if using an older version)
     - `CustomItems.dll` (if available)
   - From **ShadowLib**:
     - `ShadowLib.dll`
     - `lstwo.shadowlib`
     - `UniverseLib.Mono.dll`

   Your `BepInEx/plugins` folder should look like this:
   ```
   Wobbly Life/BepInEx/plugins
     ├── UniverseLib.Mono.dll
     ├── CustomItems.dll
     ├── lstwo.shadowlib
     ├── lstwoMODS.dll / NotAzzamods.dll
     └── ShadowLib.dll
   ```

## Step 5: Launch the Game
- Run Wobbly Life. BepInEx should load the mod automatically.

## Troubleshooting
- If the mod does not load, ensure the files are in the correct `BepInEx/plugins` folder.
- Verify that you are using **BepInEx 5 Mono** and **UniverseLib Mono** (not IL2CPP).
- Check the BepInEx logs in `BepInEx/LogOutput.log` for any error messages.
- If it still doesn't load submit an issue [here](https://github.com/lstwo/lstwoMODS/issues)
  
# Mod List

- **Player Mods (can apply to any player)**
  - Character Manager
  - Controller Manager
  - Frog Mods
  - Ragdoll Manager
  - Smite Player
  - Teleport All Players
  - Change Player Name
  - Complete Job
  - Movemenet Manager
  - Clothing Manager (only for yourself)
  - Give Money (only for yourself)

- **Vehicle Mods (can apply to any player)**
  - Enter Exit Interact Modifier
  - Road Vehicle Modifier

- **Server Mods (applies to all players)**
  - Ragdoll All Players
  - Server Settings
  - Set Time
  - Prevent Drowning
  - Set Gravity
  - Weather Editor (thunder doesn't work)

- **Save File Mods (applies only to you)**
  - Museum Manager
  - Mission Completer
  - Present Manager
  - Achievement Manager

- **Extra Mods**
  - Accurate Physics Mode
  - Banana Peel Backpack Modifier
  - Cyberpunk Mode
  - Debt
  - Jetpack Multiplier
  - Realistic Car Crashes
  - Buy Unlimited Houses (doesn't always fully work)
  - First Person
  - Hide UI

# Building Yourself

If you want to get the latest and most unfinished features you can try to build it yourself.

1. Clone the repository
2. Open it in Visual Studio (or any other IDE / compiler)
3. Build the Project
4. Copy the lstwoMODS.dll from `<Project Folder>/bin/Debug/net46/` to `<Game Folder>/BepInEx/plugins/`

# FAQ

- **Does it have a server player count changer?**

  No, just use [Larger Lobbies](https://www.nexusmods.com/wobblylife/mods/8) for that.

- **Why did you change the name? (No one actually asked that)**

  Because "Not Azzamods" is very confusing at times.
