# grub2-theme-aether
Simple GRUB theme inspired by the lightdm-webkit2 theme [Aether](https://github.com/NoiSek/Aether).

***
## Table of contents
- [Design](#design)
- [Installation](#installation)
- [Credits](#credits)

***
## Design
![](../screenshots/demo.gif)

These colours were used for the following images:
| Files | Colour (Hex) | Alpha |
| ----- | ------------ | ----- |
| boot_menu_*.png | #7AD7F0 | 0.6 |
| select_*.png | #072D40 | 0.5 |
| slider_*.png | #6BBBE1 | 0.8 |

## Installation
1. Clone this repository to `/usr/share/grub/themes/grub2-theme-aether`
2. Open the GRUB config at `/etc/default/grub` and set the value of `GRUB_THEME` to the path of the theme\`s `theme.txt`:
   ```
   GRUB_THEME="/usr/share/grub/themes/grub2-theme-aether/theme.txt"
   ```
   (Also make sure to comment the option `GRUB_TERMINAL_OUTPUT`, otherwise the graphical terminal will be disabled)
3. Update the GRUB config using your distros update grub command.
   | Distro | Command |
   | ------ | ------- |
   | Debian (pre 10), Ubuntu | update-grub |   
   | Debian 10+, Arch   | grub-mkconfig -o /boot/grub/grub.cfg |
   | Fedora | grub2-mkconfig -o /boot/efi/EFI/fedora/grub.cfg |

## Credits
- Terminus Font by Dimitar Toshkov Zhekov
- Linux distro & BSD icons from official downloads
- Shutdown & reboot icons & background from [Aether](https://github.com/NoiSek/Aether)
- Console icon from [Flat-Remix](https://github.com/daniruiz/flat-remix)
