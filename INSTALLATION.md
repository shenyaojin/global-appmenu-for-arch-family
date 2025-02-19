Installation
============

## Using installation script

**Before running the installation script you have to install the dependencies needed for compiling.**


### KDE Neon / Ubuntu

```
sudo apt install make cmake extra-cmake-modules qtdeclarative5-dev libkf5plasma-dev libqt5x11extras5-dev g++ libsm-dev libkf5configwidgets-dev libkdecorations2-dev libxcb-randr0-dev libkf5wayland-dev plasma-workspace-dev
```

### openSUSE Leap 15 / Tumbleweed

```
sudo zypper in -y xrandr cmake make gcc gcc-c++ extra-cmake-modules libqt5-qtbase-devel libqt5-qtdeclarative-devel libKF5WindowSystem5 plasma-framework-devel libSM-devel libqt5-qtx11extras-devel libkdecoration2-devel kconfigwidgets-devel kwidgetsaddons-devel kdeclarative-devel
```

### Fedora
```
sudo dnf install make cmake extra-cmake-modules qt5-qtdeclarative-devel kf5-plasma-devel qt5-qtx11extras-devel gcc-c++ libSM-devel kf5-kconfigwidgets-devel kdecoration-devel kf5-kitemmodels-devel plasma-workspace-devel kf5-kwayland-devel 
```

### Arch

```
sudo pacman -Sy base-devel libxcb plasma-workspace qt5-base qt5-declarative extra-cmake-modules kwindowsystem plasma-framework libdbusmenu-gtk2 libdbusmenu-gtk3
```

Change the KDE_INSTALL_QMLDIR value to /usr/lib/qml: 

```
vim ~/.zshrc
```

Add the variable: 
```
export KDE_INSTALL_QMLDIR="/usr/lib/qml:$KDE_INSTALL_QMLDIR"
```

then reboot or log in the account again.

### Building and Installing

**Now you can run the installation script.**

```
sh install.sh
```

