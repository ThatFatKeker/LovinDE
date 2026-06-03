# LovinDE 🚀
A remaster to my plainDE installer script

An automated bash script designed to install and configure the **Openbox** window manager and overlay it with **plainDE** components on a fresh **Arch Linux** installation. It handles system updates, dependencies, AUR helper setup, and custom UI components in one click.

---

## Features

* **Full Graphical Stack Setup:** Installs `Xorg-server`, `xinit`, and `Openbox`.
* **AUR Helper Integration:** Automatically clones and builds `yay-bin` for AUR access.
* **plainDE Implementation:** Installs `plainde-meta-git` and core graphical system elements.
* **Automatic Config Handling:** Deploys clean environment configs and links the plainDE desktop panel and control center (`plainpanel`, `plaincontrolcenter`) straight to the Openbox autostart sequence.
* **Aesthetics Included:** Bundles basic font configurations (`ttf-dejavu`, etc.) and system audio utilities (`pipewire`).

---

## What It Installs

* **Base Desktop:** `openbox`, `obconf`, `xorg-server`, `xorg-xinit`, `xterm`
* **AUR Helper:** `yay`
* **plainDE Core:** `plainde-meta-git`, `plaincontrolcenter-git`
* **Theming & Media:** `lxappearance-gtk3`, `arc-gtk-theme`, `papirus-icon-theme`, `pipewire`, `wireplumber` `alsa-utils`

---

## How to Use

> ⚠️ **Warning:** This script targets **Arch Linux**. Run it on a fresh installation or an environment where you want to deploy Openbox + plainDE.

### 1. Clone the repository
```bash
git clone https://github.com/ThatFatKeker/LovinDE
cd LovinDE
```

### 2. Make the script executable
```bash
chmod +x LovinDE.sh
```

### 3. Run the installer
```bash
./Code.sh
```

### 4. Boot into your new desktop
After the installation completes successfully, launch your new environment by executing:
```bash
startx
```

---

## Post-Installation Configuration

* Use **`plaincontrolcenter`** (accessible from your system tray or menu) to manage system layouts and preferences.
* Use **`lxappearance`** to change application themes, icon styles, and default system cursors.

---

## License

This project is licensed under the **MIT License** — see the [LICENSE](LICENSE) file for details.
