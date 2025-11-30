<div align="center">

# 🛠️ modinfo.ini Maker

<img src="https://img.shields.io/badge/version-0.9.1-00f0ff?style=for-the-badge" alt="Version">
<img src="https://img.shields.io/badge/platform-Windows-0078D6?style=for-the-badge&logo=windows" alt="Platform">
<img src="https://img.shields.io/badge/Electron-latest-47848F?style=for-the-badge&logo=electron" alt="Electron">
<img src="https://img.shields.io/badge/license-MIT-00ff41?style=for-the-badge" alt="License">

**A visual tool for creating modinfo.ini files for Cyberpunk 2077 mods**

Part of the [Cyberpunk 2077 Mod Manager](https://github.com/TheCuteFatCat/Cyberpunk-2077-Modmanager) ecosystem

[Features](#✨-features) • [Installation](#🚀-installation) • [Usage](#📖-usage) • [File Format](#📋-file-format)

---

</div>

## 📝 About

The **modinfo.ini Maker** is a companion tool for the Cyberpunk 2077 Mod Manager that simplifies the creation of `modinfo.ini` files. These files provide metadata about your mods, enabling features like:

- Rich mod descriptions and screenshots
- Author attribution with Nexus Mods profile links
- Dependency tracking
- In-game item and vehicle spawn codes
- Add-on relationships

### ✨ Features
- **Auto-Save Folder Location** - Remembers your mod folder for quick exports
- **Load & Edit** - Open existing modinfo.ini files for modification
- **Multiple Authors** - Support for up to 2 mod authors
- **Dependency Manager** - Add multiple required mods with ease
- **Code Formatter** - Automatically formats console commands

---

## 🚀 Installation

### Download Release
1. Download the latest release from [Releases](https://github.com/TheCuteFatCat/INIMAKER/releases)
2. Run the installer or portable executable
3. Launch the application
   
```

---

## 📖 Usage

### First Time Setup

1. **Set Mod Folder** (Optional)
   - Click the ⚙️ **Ordner** button in the header
   - Select the parent folder containing your mod folders
   - This allows the tool to automatically find the correct mod folder when saving

### Creating a modinfo.ini

1. **Fill Out the Form**
   - Enter your mod's name, version, and description
   - Add author information (Nexus Mods username)
   - Select a category from the dropdown
   - Enter the Nexus Mods mod number (from the URL)

2. **Add Dependencies** (Optional)
   - Enter required mods like "ArchiveXL" or "Cyber Engine Tweaks"
   - Click **+** to add more requirements
   - Click **−** to remove a requirement

3. **Add Item Codes** (Optional)
   - Enter console commands for spawning items
   - One code per line, for example:
     ```
     Game.AddToInventory("Items.YourItem_01")
     Game.AddToInventory("Items.YourItem_02")
     ```
   - Semicolons are automatically removed

4. **Preview Your Work**
   - Click the **Preview** button to see the formatted output
   - Check that all information is correct

5. **Save the File**
   - Click **Save as modinfo.ini**
   - If you set a mod folder, the tool will try to find your mod automatically
   - Otherwise, select the destination folder manually
   - The file will be saved as `modinfo.ini`

### Editing an Existing File

1. Click the 📂 **Load** button in the header
2. Select your existing `modinfo.ini` file
3. All fields will be populated automatically
4. Make your changes and save

---

## 📋 File Format

The tool generates `modinfo.ini` files with the following structure:

```ini
name=My Awesome Mod
addonfor=Main Mod Name
version=1.0
description=A cool new outfit for V
screenshot=screen.png
author=YourNexusUsername
authorlink=https://next.nexusmods.com/profile/YourNexusUsername
author2=Contributor
authorlink2=https://next.nexusmods.com/profile/Contributor
category=Armour and Clothing
modlink=https://www.nexusmods.com/cyberpunk2077/mods/12345
requirements=ArchiveXL, Cyber Engine Tweaks
codes=Game.AddToInventory("Items.MyItem_01")Game.AddToInventory("Items.MyItem_02")
```

### Field Reference

| Field | Required | Description |
|-------|----------|-------------|
| `name` | ✅ | Display name of your mod |
| `addonfor` | ✅ | Parent mod name (if this is an add-on) |
| `version` | ⚠️ Recommended | Version number |
| `description` | ⚠️ Recommended | Brief description |
| `screenshot` | ❌ | Screenshot filename (defaults to `screen.png`) |
| `author` | ✅ | Primary author's Nexus username |
| `authorlink` | ✅ | Auto-generated Nexus profile URL |
| `author2` | ❌ | Second author (optional) |
| `authorlink2` | ❌ | Second author's profile URL |
| `category` | ✅ | Mod category |
| `modlink` | ✅ | Auto-generated from mod number |
| `requirements` | ❌ | Comma-separated list of required mods |
| `codes` | ❌ | Console commands for spawning items |

### Valid Categories
- Appearance
- Armour and Clothing
- Characters
- Gameplay
- Miscellaneous
- Modders Resources
- User Interface
- Utilities
- Vehicles
- Visuals and Graphics
- Weapons
- Framework

---

## 🎯 Why Use This Tool?

### For Mod Creators
- **Save Time** - No more manual text file editing
- **Reduce Errors** - Validation ensures correct format
- **Professional Results** - Properly formatted links and metadata
- **Easy Updates** - Load and modify existing files quickly

### For the Community
- **Better Mod Manager Integration** - Enables rich features in the Mod Manager
- **Improved Discoverability** - Proper categorization and metadata
- **Clear Dependencies** - Users know exactly what's required
- **Item Code Reference** - Easy access to spawn commands

---

## 🔗 Related Projects

This tool is part of the **Cyberpunk 2077 Mod Manager** ecosystem:

- **[Cyberpunk 2077 Mod Manager](https://github.com/TheCuteFatCat/Cyberpunk-2077-Modmanager)** - Main mod management application
- **[Community modinfo.ini Collection](https://justpaste.it/mawx0)** - Pre-made files for popular mods

---

## 🤝 Contributing

Contributions are welcome! Please feel free to submit a Pull Request.

### Development Setup
```bash
npm install
npm start
```

### Building
```bash
npm run build          # Build for current platform
npm run build-win      # Windows installer
npm run build-portable # Portable executable
```

---

## 📄 License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

---

## 🙏 Acknowledgments

- CD Projekt Red for Cyberpunk 2077
- The Nexus Mods community
- All mod creators making Night City even better

---

<div align="center">

**Made with ❤️ for the Cyberpunk 2077 modding community**

⭐ Star this repo if you find it useful!

</div>
