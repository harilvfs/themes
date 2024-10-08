# Theme Collection

A collection of themes compatible with Linux window managers and desktops.

## Installation Instructions

### 1. Clone the Repository
First, clone this repository to your local machine:
```bash
git clone https://github.com/harilvfs/themes
```

### 2. Change to the Cloned Directory
Navigate into the directory that contains the themes:
```
cd themes
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
