### Change Log

---

###### 2019.01.11

- `archlabs-scripts` version update

- `archlabs-polybar` has been upgraded to the latest [release](https://github.com/jaagr/polybar/releases)

- `xdg-user-dirs` is now installed for WM during install

- `archlabs-installer` version update with bug fixes and improvements

---

###### 2018.12.17

- archlabs-installer has gone from version 1.6.19 to 1.8.1 with well over 100 commits since

- no graphical live environment, you’re dropped into the console and go from there

- `aurman` has been removed and replaced with `baph`, a more minimal and simple AUR helper

- archlabs-polybar now ships `/etc/skel/.config/polybar` and the scripts used in the modules

- `archlabs-user-skel` was removed and split up into `archlabs-skel-base` and `archlabs-skel-WM_NAME` packages to accommodate the new options during install

- `aurman`, `al-hello`, `nvidia-installer`, `ob-autostart`, and possibly a few other packages have been removed and are no longer supported

- archlabs-pipemenus has been split into two separate packages `archlabs-pipemenus` and `archlabs-scripts` the first contains only pipemenus used in the openbox session, scripts contains some generic helpers including: `al-compositor`, `al-polybar-session`, `al-info`, `baph`, `flash`, and `session-logout`

- al-obkey got a minor patch to fix `XF86Audio` and `XF86Backlight` dedicated keys

- large number of what we would call 'bloat' packages have been removed from the default install, if you require one of them simply install it like any other package

- zsh, bash, and mksh all now have directories under `~/.SHELL_NAME` with configuration, helper functions, and aliases. zsh is the most fleshed out as it's what myself and other team members use. popular framwork oh-my-zsh is a bit too bloated for us to consider it as an option so were using [zsh_simpl](https://bitbucket.org/natemaia/zsh-simpl/src/master/) which aims to be more minimal while still offering nice defaults, a few plugins, and of course the amazing completion

- for intel graphics an xorg config enabling `TearFree` is created, this avoid the need to mess with compton's vsync settings, the driver vsync is just plain better.

- logout dialog now only offers the logout option when not using autologin and xinit

- i3 got a few keybind changes/additions courtesy of @LionessAlana

- openbox menu has been cut down to accommodate the lack of pre-installed defaults while still being usable

- (neo)vim  have some additional configuration, colorscheme changes and an improved c syntax file.

- all fonts are now set to either `monospace serif sans` and these are aliased to the system fonts in `~/.config/fontconfig/fonts.conf`, this allows setting all your applications to use, say `monospace` then only need to change it in one place for all applications that use it.

- compton's config has had a few tweaks and deprecated options removed

- autostart daemons/applications used across all environments are now run in `~/.xprofile` this file will be run whether using lightdm or xinit and regardless of what WM/DE, this makes running things like polkit easier for us, rather than having to keep each command up to date in each WM config etc.

---

