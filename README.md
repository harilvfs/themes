## Theme Collection

A collection of themes compatible with Linux window managers and desktops.

## Installation

### Clone the Repository
```bash
git clone https://github.com/harilvfs/themes
```

### Change to the Cloned Directory
```
cd themes/
```

### 3. Install the Themes

You have two options to install the themes:

#### Option 1: System-Wide Installation
Move all the themes to the system's shared theme directory:
```
sudo mv * /usr/share/themes/
```

#### Option 2: User-Specific Installation
Alternatively, you can install the themes for a single user by creating a custom directory in your home configuration:
```bash
mkdir -p ~/.config/themes
mv * ~/.config/themes/
```

## Kvantum Setup Guide

For Qt applications, **Kvantum** is used to apply themes. Here’s how to set up Kvantum with this theme collection:

### Clone the Theme Collection

```bash
git clone https://github.com/harilvfs/themes
```

### Change to the themes dir

```bash
cd themes/
```

### Copy Kvantum Themes

```bash
cp -r Kvantum ~/.config/Kvantum
```

### Apply Kvantum Themes

Once the themes are in place, use the Kvantum Manager to select and apply the desired theme:

Open **Kvantum Manager**: You can launch it from your desktop environment or by running:

```bash
kvantummanager
```

Under the "Change/Delete Theme" tab, select the theme you want from the list and apply it.

## Package Requirements

Depending on whether you're using **X11** or **Wayland**, you’ll need to install specific packages to manage your themes.

### For X11

To apply themes on **X11**-based systems, install the following packages:

- **`lxappearance`**: A GTK theme switcher for X11 environments.
- **`kvantum-qt5`**: A theme manager for Qt5 applications (use `kvantum-qt6` for Qt6 applications).

#### Install Required Packages for X11:
```bash
sudo pacman -S lxappearance kvantum-qt5
```

*If you’re using Qt6 applications:*
```bash
sudo pacman -S kvantum-qt6
```

### For Wayland

If you are using **Wayland**, you’ll need the following packages:

- **`nwg-look`**: A GTK theme switcher for Wayland.
- **`kvantum-qt5`** or **`kvantum-qt6`**: For managing Qt applications under Wayland.

#### Install Required Packages for Wayland:
```bash
sudo pacman -S nwg-look kvantum-qt5
```

*For Qt6 applications:*
```bash
sudo pacman -S kvantum-qt6
```

## Usage

Once the themes are installed and the required packages are set up, you can apply the themes as follows:

- **For X11**: Use `lxappearance` to select and apply GTK themes, and `kvantum` for Qt themes.
- **For Wayland**: Use `nwg-look` to apply GTK themes, and `kvantum` for Qt themes.

You can also manually configure your window manager or desktop environment to apply the themes by editing the relevant configuration files.

## License

This theme collection is licensed under the MIT License. See the [LICENSE](./LICENSE) file for more details.
