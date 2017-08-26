Configs and scripts to launch a WindowMaker session with GNUstep, gnome-settings-daemon, conky and compton as compositing manager. A Windowmaker theme, a Gnome theme and an icontheme are also provided so that the look will be more coherent with GNUstep's Rik.theme.

The windowmaker theme is a modifyed version of the Rhaps theme from https://www.opendesktop.org/s/Window-Managers/p/1018322/. You should put this Rik.themed in .../Library/WindowMaker/Themes.

GnomeRikIcons-master is based on GnomeYosemiteIcons-master from https://raw.githubusercontent.com/ActusOS/GnomeYosemiteIcons

myDF-Arc-OSX is a modified version of DF-Arc-OSX at https://www.gnome-look.org/content/show.php/Arc-OSX-themes?content=175536.



- autostart must be copied into your ~/GNUstep/Library/Windowmaker directory.
- you can disable conky, compton or gnome-settings-daemon in it by commenting them out.
- compton.conf must be copied into ~/.config/ directory.
- conkyrc must be renamed ~/.conkyrc
- Rik.themed is to be put in  ~/GNUstep/Library/Windowmaker/Themes.You will be able to select it with Windowmaker desktop menu.
- GnomeRikIcons-master is to be put in /usr/share/icons or in ~/local/share/icons
- myDF-Arc-OSX goes to /usr/share/themes or in ~/share/themes.
- you can use Gnome-tweak-tool to use GnomeRikIcons-master and myDF-Arc-OSX in gnome-apps.

