# myAwesomewm
This is my awesome WM config files.

## Based on
Awesome WM theme used copycat-killer's awesome WM theme collection.
[See here](https://github.com/copycat-killer/awesome-copycats)

## `.xprofile` content
```shell
!/bin/sh
#fcitx need
export XMODIFIERS=@im=fcitx
export QT_IM_MODULE=fcitx
export GTK_IM_MODULE=fcitx
fcitx-autostart

gnome-settings-daemon &
gnome-power-manager &
xcompmgr -c &
nm-applet --sm-disable &
update-notifier &

# shadowsocks need
ss-qt5 &
sh start-kcptun.sh &

# !!! change this as suit your condition !!!
# use xrandr to show specified infos of your monitors
xrandr --output HDMI-1 --above eDP-1

exec awesome
```

