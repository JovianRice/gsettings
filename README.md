
# Useful gsettings commands

Here are a few gsettings commands that I have found useful. 

Allow volume to go above 100 (over-amplification)

```gsettings set org.gnome.desktop.sound allow-volume-above-100-percent 'true'```

Disable animations

```gsettings set org.gnome.desktop.interface enable-animations false```

Disable location services

```gsettings set org.gnome.system.location enabled false```

Disable recent files

```gsettings set org.gnome.desktop.privacy remember-recent-files false```

```rm ~/.local/share/recently-used.xbel```

Disable hot corner

```gsettings set org.gnome.desktop.interface enable-hot-corners false```

Replace "switch applications" with "switch windows" (the way Alt+Tab is supposed to work)

```gsettings set org.gnome.desktop.wm.keybindings switch-applications "[]"```

```gsettings set org.gnome.desktop.wm.keybindings switch-windows "['<Alt>Tab']"```

Super+Tab to show the overview (instead of Super+S)

```gsettings set org.gnome.shell.keybindings toggle-overview "['<Super>Tab']"```

Minimize, maximize buttons in windows

```gsettings set org.gnome.desktop.wm.preferences button-layout "appmenu:minimize,maximize,close"```

Dark theme (new gnome thing in Settngs>Appearance)

```gsettings set org.gnome.desktop.interface color-scheme "prefer-dark"```

Make night light manual (0:00-0:00), set temperature (lower = more orange), enable it

```gsettings set org.gnome.settings-daemon.plugins.color night-light-schedule-from 0```

```gsettings set org.gnome.settings-daemon.plugins.color night-light-schedule-to 0```

```gsettings set org.gnome.settings-daemon.plugins.color night-light-schedule-automatic false```

```gsettings set org.gnome.settings-daemon.plugins.color night-light-temperature 2700```

```gsettings set org.gnome.settings-daemon.plugins.color night-light-enabled true```

Disable searching for anything but your installed applications

```gsettings set org.gnome.desktop.search-providers disable-external true```

Workspaces to apply to all monitors (else if you have an app on your second monitor it will remain when you switch)

```gsettings set org.gnome.mutter workspaces-only-on-primary false```
