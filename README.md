# What Is This?
This the EFI folder of my current hackintosh setup on my Acer Swift 3 (EU Version). Since there isn't any setup guides for the EU version of this device, I have decided to upload my own configuration. I am currently dealing with university applications, don't have enough time to debug my opencore setup so for a while the releases will depend on Clover Bootloader in order to protect the stability of the overall system.

# How To Install?
 - Create an installation disk via [createinstallmedia](https://support.apple.com/en-us/HT201372) method
 - Download the EFI Folder
 - Download the following softwares 

> headkaze's [Hackintool](https://github.com/headkaze/Hackintool)

> corptnewt's [ProperTree](https://github.com/corpnewt/ProperTree) and [MountEFI](https://github.com/corpnewt/MountEFI)

 - Use the hackintool to get a serial number and a following board number that fits with the model **MacBookPro14,2** (This is important, setups based on other models' codes don't work well)
 - Edit the **config.plist** according to your preferences (Themes, Timeout e.g.) and put the acquired numbers into the **SMBIOS** section with **ProperTree**
 - Mount the installation disk's **EFI** partition via **MountEFI**
 - Drop the modified **EFI** folder into the disk's **EFI** partition
 - Boot into **BIOS** and do the installation
 - ***Congratulations! You now have working system, but we are not done yet.***
 - Mount the **EFI** partitions of the both disks and transfer the **EFI** folder of flash drive to your system's main drive
 - In **Terminal**, type the following : `sudo spctl --master-disable`
 - In **Finder > Preferences > General >** Select to show hard disks on the desktop
 - In **System Preferences > User and groups**
    - Click on the lock and type your password
    - Click on Login Options and select your user in Automatic login
## Recommended Programs For A Better Experience
 - [MOS](https://github.com/Caldis/Mos) (Smooth Scrolling Enabler)
 - [OpenMTP](https://github.com/ganeshrvel/openmtp) (Mounter for Android Phones)
 - [Homebrew](https://brew.sh/) (Package Installer for macOS)
 - [VLC](https://www.videolan.org/vlc/index.html) (Open-source Video Player, cause QuickTime sucks hard)

## ***This version is NOT TESTED on macOS 10.15.3***
