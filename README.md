# genpkg
stupid simple but customizable dmenu/shell script which opens the Gentoo wiki for an ebuild

## Preview
![image](https://github.com/speediegamer/genpkg/blob/images/genpkg_dmenu.gif?raw=true)

## Usage (dmenu)
Install the script (see installation) and run it using dmenu. Make sure to edit the config file to match your system.

## Usage (terminal)
Install the script (see installation) and run it inside a terminal. Make sure to edit the config file to match your system and disable dmenu support.

## Installation
Download the [script](https://raw.githubusercontent.com/speediegamer/genpkg/main/genpkg) and save it to /usr/bin, /usr/local/bin, or any other path specified in your shell's $PATH variable. Then chmod +x it to make sure it's executable.

If /bin/sh isn't an alias then edit the script and change #!/bin/sh to a shell on your Linux system.
The script will NOT run without a configuration file to unless you feel like writing the entire thing from scratch follow Configuration.

## Notes
- This script has dependencies on Gentoo based distributions and will NOT work if Portage (gentoo package manager) is not available.
- Rofi support might become a patch later on.
- Support for other distributions might become a patch later on.
- On some Gentoo based distributions, /etc/portage/make.conf is not present. If so, replace it in the script with YOUR make.conf.

## Configuration
Create ~/.config/genpkg and save [this](https://raw.githubusercontent.com/speediegamer/genpkg/main/genpkgrc) file to ~/.config/genpkg/genpkgrc. Now change these variables to what's present on your system:
- GENPKG_BROWSER (set this to a web browser available on your system. Works best with terminal web browsers)
- GENPKG_GENTOO (change this if you're using funtoo or something like that, otherwise leave as default)
- GENPKG_USEDMENU (set this to 'true' if you will be using dmenu, 'false' if you will not)
- GENPKG_DMENU_PATH (set this to the full path to the dmenu binary on your system.
- GENPKG_DMENU_TERMINAL (set this to the full path to the terminal binary on your system)

## Credits
Me, me me. Who else? No one.

## Have issues?
Report any issues to the GitHub page Issues.
