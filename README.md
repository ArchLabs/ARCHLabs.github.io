### RELEASE NOTES
---
###### 2022.08.21
- ArchLabs Release, 2022.05.29 is available for download [LTS Kernel](https://sourceforge.net/projects/archlabs-linux-minimo/files/ArchLabsMinimo/archlabs-lts-2022.08.21-x86_64.iso/download) - [Vanilla Kernel](https://sourceforge.net/projects/archlabs-linux-minimo/files/ArchLabsMinimo/archlabs-2022.08.21-x86_64.iso/download).

- Added basic live session for dk.

- Update session skeleton configs.

- General updates - latest archiso, kernel, firmware, etc.

- Replace exo-open with scripts for default applications (terminal, browser, and file manager).

- Remove ksuperkey and the whole XFCE suite in favour of lxappearance.

- Update openbox pipemenu scripts and remove old unused ones.

- Update kickshaw (openbox menu editor) to be inline with upstream.

- Update dk session lemonbar script with better DPI support and more info.

- Simplify and merge some menus/descriptions.

- General clean up and remove dead/unused packages.

- Reduce number of sessions to dk, openbox, i3-gaps, bspwm, and fluxbox.

- Remove refind (bootloader), sddm, and gdm (display managers).

- Remove -t flag. AMD and Intel will have TearFree xorg configs setup by default.

- Remove nvidia-installer for nvidia driver setup during install.

- Added gpg signed checksum files for ISOs, use gpg --verify and sha256sum -c to confirm the ISO checksum. 

---
###### 2022.05.29
- ArchLabs Release, 2022.05.29 is available for download [LTS Kernel](https://sourceforge.net/projects/archlabs-linux-minimo/files/ArchLabsMinimo/archlabs-lts-2022.05.29-x86_64.iso/download) - [Vanilla Kernel](https://sourceforge.net/projects/archlabs-linux-minimo/files/ArchLabsMinimo/archlabs-2022.05.29-x86_64.iso/download).

- Update to the Sway session:
	
	- sway session comes with nwg-shell 0.2

	- Now includes it's own tools to manage outputs (nwg-displays instead of wdisplays) and GTK settings (nwg-look instead of lxappearance).

- Minor tweaks and fixes to the installer

- Fixed volumeicon tray application mixer button

- Fixed broken obkey package after recent removal of python2 packages from Arch [community] repo


---
###### 2022.02.12
- ArchLabs Release, 2022.02.12 is available for download [LTS Kernel](https://sourceforge.net/projects/archlabs-linux-minimo/files/ArchLabsMinimo/archlabs-lts-2022.02.12-x86_64.iso/download) - [Vanilla Kernel](https://sourceforge.net/projects/archlabs-linux-minimo/files/ArchLabsMinimo/archlabs-2022.02.12-x86_64.iso/download).

- Update to the Sway session:

	- New notification panel.

	- Tweaks to the nwg-shell.

- The installer has been updated.

- Introduction of an LTS Kernel ISO.

- General fixes and tweaks.

- Baph has been updated to version 1.6.


---
###### 2022.01.19

- ArchLabs Release, 2022.01.18 is available for [download](https://sourceforge.net/projects/archlabs-linux-minimo/files/ArchLabsMinimo/archlabs-2022.01.18-x86_64.iso/download).

- The addition of dk and Sway window managers.

- Tweak and tidy up of XFCE4 session.

- New default wallpaper based on this [original](https://unsplash.com/photos/OzD_vkpMM5Y) by Jack Zhong.

- Updated the ArchLabs repository.

- Updated Rofi theme.

- ArchLabs AUR helper BAPH has had an update - version 1.5 brings a new check update flag and other minor improvements.


---
###### 2021.05.02

- ArchLabs Release, 2021.05.02 is available for [download](https://sourceforge.net/projects/archlabs-linux-minimo/files/ArchLabsMinimo/archlabs-2021.05.02-x86_64.iso/download).

- No major changes.

- Nate's tiling window manager, dk is available from the [AUR](https://aur.archlinux.org/packages/dk/)

---

###### 2020.11.04

- Archlabs Release, 2020.11.04 is available for [download](https://sourceforge.net/projects/archlabs-linux-minimo/).

- Usual updates to the `archlabs-installer` and minor changes.

- The `archlabs-installer` has been moved directly to the ISO rather than be supplied as an extra package.

- First ArchLabs release built with the new Archiso build process.

---
###### 2020.05.04

- ArchLabs release, 2020.05.04 is available for [download](https://sourceforge.net/projects/archlabs-linux-minimo/).

- `archlabs-installer` has had some updates and improvements.  Now at version `2.1.45`.

  - The installer now optionally uses Pacstrap to install packages.

  - The installer is more portable than ever.

  - General bug fixes.

- Packages Updates.

- The Rofi script has had a slight update.

- Updates to `baph` our AUR helper. `man baph` for details on how to use `baph`.

- Adwaita-Dark is now the default GTK theme where applicable.

- LXQT added to the list of install options.

- May the Fourth Be With You.

---

###### 2019.10.28

- `archlabs-installer` has been updated to version `2.1`.

	- the installer won't gobble stderr when redirecting it for error handling

	- live session setup flag + more *(see --help)*

	- live session now available.  instructions are available when you boot the iso.

	- jwm has been added as option to the wm/de install.

- updated wallpaper, a slice of home for dobbie.  

	- original wallpaper found [here](https://unsplash.com/photos/RxBA85tbj-c).

	- custom wallpapers from the community can be downloaded [here](https://bitbucket.org/archlabslinux/custom-al-wallpapers/src/master/)

- overhauled UI by the way of updated themes.  

	- original theme by [lassekongo83](https://www.deviantart.com/lassekongo83/art/Stilo-themes-796881403) from deviantart.

- `tint2` has replaced `polybar` as the default panel in the openbox and bspwm sessions. 

	- jgmenu is the tint2 application launcher. 

	- i3wm and dwm use their respective default status bars

- `baph` our in house `aur` helper is now its own package.

- general improvements and bug fixes


---

###### 2019.01.20

- `archlabs-scripts` version update.

- `archlabs-polybar` has been upgraded to the latest [release](https://github.com/jaagr/polybar/releases).

- `xdg-user-dirs` is now installed for WM during install.

- `archlabs-installer` version update with bug fixes and improvements.

---

###### 2018.12.17

- archlabs-installer has gone from version 1.6.19 to 1.8.1 with well over 100 commits since.

- no graphical live environment, you’re dropped into the console and go from there.

- `aurman` has been removed and replaced with `baph`, a more minimal and simple AUR helper.

- archlabs-polybar now ships `/etc/skel/.config/polybar` and the scripts used in the modules.

- `archlabs-user-skel` was removed and split up into `archlabs-skel-base` and `archlabs-skel-WM_NAME` packages to accommodate the new options during install.

- `aurman`, `al-hello`, `nvidia-installer`, `ob-autostart`, and possibly a few other packages have been removed and are no longer supported.

- archlabs-pipemenus has been split into two separate packages `archlabs-pipemenus` and `archlabs-scripts` the first contains only pipemenus used in the openbox session, scripts contains some generic helpers including: `al-compositor`, `al-polybar-session`, `al-info`, `baph`, `flash`, and `session-logout`.

- al-obkey got a minor patch to fix `XF86Audio` and `XF86Backlight` dedicated keys.

- large number of what we would call 'bloat' packages have been removed from the default install, if you require one of them simply install it like any other package.

- zsh, bash, and mksh all now have directories under `~/.SHELL_NAME` with configuration, helper functions, and aliases. zsh is the most fleshed out as it's what myself and other team members use. popular framwork oh-my-zsh is a bit too bloated for us to consider it as an option so were using [zsh_simpl](https://bitbucket.org/natemaia/zsh-simpl/src/master/) which aims to be more minimal while still offering nice defaults, a few plugins, and of course the amazing completion.

- for intel graphics an xorg config enabling `TearFree` is created, this avoid the need to mess with compton's vsync settings, the driver vsync is just plain better.

- logout dialog now only offers the logout option when not using autologin and xinit.

- i3 got a few keybind changes/additions courtesy of _LionessAlana_.

- openbox menu has been cut down to accommodate the lack of pre-installed defaults while still being usable.

- (neo)vim  have some additional configuration, colorscheme changes and an improved c syntax file.

- all fonts are now set to either `monospace serif sans` and these are aliased to the system fonts in `~/.config/fontconfig/fonts.conf`, this allows setting all your applications to use, say `monospace` then only need to change it in one place for all applications that use it.

- compton's config has had a few tweaks and deprecated options removed.

- autostart daemons/applications used across all environments are now run in `~/.xprofile` this file will be run whether using lightdm or xinit and regardless of what WM/DE, this makes running things like polkit easier for us, rather than having to keep each command up to date in each WM config etc.

---

