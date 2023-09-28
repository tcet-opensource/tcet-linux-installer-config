# TCET Linux Installer Config

This repository contains the source code for the configuration of the calamares installer provided to install TCET-Linux.

## Config structure

```
─ calamares
 ├── branding
 │  └── tcetlinux
 ├── modules
 │  ├── initcpio.conf
 │  ├── mount.conf
 │  ├── packages.conf
 │  ├── partition.conf
 │  ├── removeuser.conf
 │  ├── shellprocess-remove-livecd.conf
 │  ├── shellprocess-tl-mkinitcpio.conf
 │  ├── unpackfs.conf
 │  ├── users.conf
 │  └── welcome.conf
 └── settings.conf
```

The `etc/calamares` folder contains all the configurations.

It contains the following folders and files.

- **branding** : This folder is for stylizing the installer and putting appropriate pictures to the calamarees slideshow

- **modules** : This folder contains the config for all the modules we provide in the installer. The modules are as follows:

  1. **initcpio.conf** : This module is responsible for creating an initial ramdisk environment during the installation process using mkinitcpio.
  2. **mount.conf** : This module is responsible for handling the mounting of filesystems during the installation process.
  3. **packages.conf** : This module is responsible for package management during the installation process.
  4. **partition.conf** : This module is used to handle partitioning during the installation process.
  5. **removeuser.conf** : This module is used to remove a user from the system during the installation process.
  6. **shellprocess-remove-livecd.conf** : This module is used to execute shell commands in the target system during the installation process.
  7. **shellprocess-tl-mkinitcpio.conf** : This module prepares the system for installation of TCET-Linux.
  8. **unpackfs.conf** : This module is used to unpack a filesystem during the installation process.
  9. **users.conf:** : This module is used to handle user creation and configuration during the installation process.
  10. **welcome.conf** : This module is used to handle the welcome page during the installation process.

- **settings.conf** : This configuration file is for Calamares, an independent and distro-agnostic system installer for Linux distributions.

### Important links

- [tcet-linux-pkgbuild](https://github.com/tcet-opensource/tcet-linux-pkgbuild/tree/main/installer)
