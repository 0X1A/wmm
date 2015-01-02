# wmm
Window Manager Manager

Replaces the cruft in your xinitrc. Configuration goes in `~/.config/wmm/wmm.yml`
and is written in YAML.

**Example config:**
```
wm: bspwm
exec:
        - sxhkd
        - dmenu-cache 10m
        - sh ~/.fehbg
        - xrdb -merge ~/.Xresources
panel: panel
```

**Example xinitrc:**
```
wmm
```

## Installing
`gem install wmm`
