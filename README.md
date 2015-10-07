# Kali Linux Menu for Openbox

If you use Kali Linux with Openbox and want to have the nice tools menu including icons, then you can grab it here.

**UPDATE:**

Another version without icons is available as well.



## Requirements

`rxvt-unicode` package is required


## Installation

### 1. Edit `~/.config/openbox/rc.conf`

Find the `<menu>` Section (near bottom) and place `<file>menu_kali.xml</file>` somewhere into it.
```xml
<openbox_config>
	<menu>
		...
		<file>kali_menu.xml</file>
		...
	</menu>
</openbox_config>
```

### 2. Edit `~/.config/openbox/menu.xml`

Place the following line at the position of the `menu.xml` where you want the kali menu to appear.
```xml
	<menu icon=".config/openbox/icons/kali_menu/kali-menu.png" id="/Kali"/>
```
Or for the icon-less variant:
```xml
	<menu id="/Kali"/>
```


### 3. Copy files

* Copy `kali_menu.xml` (with icons) or `kali_menu-no_icons.xml` (without icons) to `~/.config/openbox/kali_menu.xml`
* Copy `icons` folder to `~/.config/openbox` so that it looks like:

```
~/.config/openbox/icons/kali_menu
```



## Note

Currently under development...
If you want to contribute, feel free.



## Todo

- [X] Finish menus
- [X] Finish submenus
- [ ] Finish launchers
- [ ] Finalize install instructions
- [ ] Make opened terminal default to system settings
