<h3 align="center">
<img width="1920" height="1080" alt="ModLoader" src="https://github.com/user-attachments/assets/a6759353-b69b-45ef-8d03-ab93312f61cc" />

  
[![Ko-fi](https://img.shields.io/badge/Ko--fi-FF5E5B?logo=ko-fi&logoColor=white)](https://ko-fi.com/thatmfrick)
![Bash Script](https://img.shields.io/badge/bash_script-%23121011.svg?style=for-the-badge&logo=gnu-bash&logoColor=white)
![Linux](https://img.shields.io/badge/Linux-FCC624?style=for-the-badge&logo=linux&logoColor=black)
![macOS](https://img.shields.io/badge/mac%20os-000000?style=for-the-badge&logo=macos&logoColor=F0F0F0)
![Android](https://img.shields.io/badge/Android-3DDC84?style=for-the-badge&logo=android&logoColor=white)

</h3>

<p align="center">
  <strong>A powerful CLI for installing, previewing, backing up, and restoring mods for World of Tanks Blitz — with zero hassle.</strong>
</p>



https://github.com/user-attachments/assets/380814ba-6951-4fa1-8cde-93f02ff6ae20



---

## ✨ Features

- ⚒️ Install various mod types — from tank models to UI enhancements
- 👀 Preview mods with links to original sources
- 📁 Auto-backup of game files before every mod install
- ♻️ Restore individual or all game files to stock
- 💻 Multi-platform support: Android, Linux and MacOs
- 🔁 Switch game platform/client info via in-app option (**Steam Wargaming/Android Wargaming only** for now)

---

## 📦 Pre-installation

### 🍎 macOS

1. Install [Homebrew]([https://brew.sh/](https://github.com/Homebrew/brew/releases)) latest release, scroll down and download the `Homebrew.pkg` file.
2. From the Downloads folder open `Homebrew.pkg` and follow the installation steps.

### 🤖 Android

The CLI offers the possibility to install modifications on Android (it requires a Linux pc with the tool installed)

1. Enable **Developer Options** on your Android device.
2. In the Developer Options menu, enable **USB debugging**.
   - **Important**: disable **any** revoke USB debugging/adb authorization timeout settings.
3. Connect your Android device to the PC, open the terminal, and run `adb devices`.
   - A pop-up will appear on your Android device — press **Trust this device** (your device is now set up).
4. Run `rickmodder` in the terminal and switch the platform to Android.

https://github.com/user-attachments/assets/f8d77724-1912-4de9-a5fd-a9340729179d

## ⚙️ Installation

Just past this in the terminal.

```bash
git clone https://github.com/RickOnGit/RickWotbMods "$HOME/RickWotbMods"
bash "$HOME/RickWotbMods/bin/setup.sh"
```

<https://github.com/user-attachments/assets/967c282c-495d-4527-99f3-cd9d755d5bcc>


## 🚀 Usage

After installation, launch the CLI with:

```bash
rickmodder
```

Use the interactive menu to browse, preview, install, and restore mods.
