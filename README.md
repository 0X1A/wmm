# wmm
Window Manager Manager

Replaces the cruft in your xinitrc. Configuration goes in `~/.config/wmm/wmm.yml`
and is written in YAML.

## Configuration Options

 Section | Description
 ------- | ----------- 
 **wm** | Window manager that will be used
 **exec** | Commands to be executed
 **background** | Commands to be executed and sent to the background
 **panel** | Command for panel

**Example config:**
```yaml
wm: bspwm
exec:
	- xrdb -merge ~/.Xresources
background:
	- sxhkd
	- dmenu-cache 10m
	- sh ~/.fehbg
panel: panel
```

**Example xinitrc:**
```bash
wmm
```

## Installing
```bash
gem install wmm
```
