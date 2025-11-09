# order
- xorg
- dwm (my git)
- alacritty (pacman)
- ttf-jetbrains-mono-nerd (pacman)
- alacritty config (my git)
- neovim (pacman)
- nvim-config (my git)
- tmux (pacman)
    + tpm (github)
- feh (pacman)
- cmatrix (github)
- fzf (pacman)
- ripgrep (pacman)
- firefox (pacman)
- dmenu (my git)
- keyd (pacman)
- zsh (pacman)
- picom (pacman)
- thunderbird (pacman)
- alsa-utils (pacman)
- pulseaudio pulseaudio-alsa (pacman)
- sxiv (pacman)
- mpv (pacman)
- newsboat (pacman)
- yt-dlp (pacman)
- acpilight (aur)
- bluez (pacman)
- bluez-utils (pacman)
- sysstat (pacman)
- libnotify (pacman)
- dunst (pacman)
- xclip (pacman)
- xdotool (pacman)
- telegram-desktop (pacman)
- zathura zathura-djvu zathura-pdf-mupdf zathura-ps (pacman)
- xorg-xrandr (pacman)

# actions
## default shell
- change default shell to zsh:
```
chsh -s /bin/zsh
```
need to re-login to take effect

## key remapping
- remap the keys, see [keyd](https://github.com/rvaiya/keyd)

## brightness control
- install [acpilight](https://aur.archlinux.org/packages/acpilight)
- allow members of video group to change the brightness file: [wiki](https://wiki.archlinux.org/title/Lenovo_ThinkPad_T480#Screen_backlight)
- add the user to the video group: `sudo usermod -aG video your_username`
- reboot the laptop
- use `xbacklight -inc/-dec $DELTA` to adjust the brightness

# TODO
- [x] fix dwmblocks
- [x] picom
- [x] mpv
- [x] newsboat
- [x] telegram
- [x] research a mail client
- [x] something to remap the fkin backspace and caps
- [ ] figure out how to make the fn keys work
    + [x] volume control
    + [x] brightness control
    + [x] bluetooth (NOTE: doesnt work)
    + [x] wifi (worked by itself)
    + [x] kb backlight
    + [ ] settings button (what is it supposed to do anyway?)
- [x] figure out why Xresources doesnt work
- [x] add to dwmblocks
    + [x] battery
    + [x] volume level
    + [x] cpu temp
    + [x] cpu load
    + [x] gpu temp? (NOTE: not available because no discrete gpu)
    + [x] number of package updates
- [x] screenshotting tool (watch bread video)
- [x] figure out why the headphones are not working; NOTE: snd_usb_audio kernel module
- [x] figure out how to test headphones' mic
- [x] figure out how to adjust headphones' volume


# useful commands
- device connection event log
```
journalctl -b --no-pager | tail -100
```
- send video to external monitor
```
xrandr --output HDMI-1 --mode 1920x1080
```
