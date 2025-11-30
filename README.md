modinfo.ini Maker
<div align="center">
<img src="https://img.shields.io/badge/version-1.0.0-00f0ff?style=for-the-badge" alt="Version">
<img src="https://img.shields.io/badge/platform-Windows-0078D6?style=for-the-badge&logo=windows" alt="Platform">
<img src="https://img.shields.io/badge/Electron-latest-47848F?style=for-the-badge&logo=electron" alt="Electron">
<img src="https://img.shields.io/badge/license-MIT-00ff41?style=for-the-badge" alt="License">
A cyberpunk-themed tool for creating modinfo.ini files for Cyberpunk 2077 mods
Companion tool for the Cyberpunk 2077 Mod Manager

</div>
🎯 What is this?
The modinfo.ini Maker helps mod creators easily generate properly formatted modinfo.ini files for their Cyberpunk 2077 mods. These files enable full compatibility with the Cyberpunk Mod Manager, unlocking features like:

Mod descriptions and author links
Screenshot displays
Item/vehicle spawn codes
Dependency tracking
Add-on detection

✨ Features

Visual Form Interface - No need to remember INI syntax
Live Preview - See your modinfo.ini as you type
Auto-formatting - Generates proper links and code formatting
Smart Validation - Highlights required fields
Load & Edit - Import existing modinfo.ini files to update them
Saved Folder - Remembers your mod folder location for quick exports

🚀 Quick Start

Download the latest release
Launch the application
Fill in your mod details in the form
Click the Preview button to verify
Save directly to your mod folder

📝 Basic Usage
First Time Setup

Click the ⚙ Ordner (Folder) button in the top-right
Select your main mods folder
The tool will remember this location

Creating a modinfo.ini

Fill in the required fields (marked with *):

Name - Your mod's name
Addon für - Parent mod name (if this is an add-on)
Autor - Your Nexus Mods username
Kategorie - Select from dropdown
Mod Nummer - Your Nexus Mods ID


Add optional information:

Version, description, screenshots
Second author (click the + button)
Required mods/dependencies
In-game spawn codes


Click Speichern als modinfo.ini (Save as modinfo.ini)

Editing an Existing File

Click 📁 Laden (Load) in the top-right
Select your modinfo.ini file
Edit any fields
Save to update the file

🎮 Code Format
When adding spawn codes, enter one per line:
Game.AddToInventory("Items.YourItem_01")
Game.AddToInventory("Items.YourItem_02")
The tool automatically formats them correctly (removes semicolons, combines into single line).
📦 Requirements

Windows 10/11
No additional software needed

🔗 Related Projects

Cyberpunk 2077 Mod Manager - The main mod manager
Community modinfo.ini Collection - Pre-made files for popular mods

🤝 For Mod Authors
Adding a modinfo.ini to your mod releases makes them fully compatible with the Mod Manager and provides a better experience for users. Consider including one in your next update!
📄 License
MIT License - see LICENSE file for details

<div align="center">
Made with ❤️ for the Cyberpunk 2077 modding community
⭐ Star this repo if you find it useful!
</div>
