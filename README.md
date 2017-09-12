Configs and scripts to launch a WindowMaker session with GNUstep, gnome-settings-daemon, conky and compton as compositing manager, and a few GNUstep apps : gdomap; gdnc, GWorkspace, AClock and a little top panel GSPanel.. A Windowmaker theme, a Gnome theme and an icontheme are also provided so that the look will be more coherent with GNUstep's rik.theme.

The windowmaker theme Rik.themed is a modifyed version of the Rhaps theme from https://www.opendesktop.org/s/Window-Managers/p/1018322/. 

GnomeRikIcons-master is based on GnomeYosemiteIcons-master from https://raw.githubusercontent.com/ActusOS/GnomeYosemiteIcons

myDF-Arc-OSX is a modified version of DF-Arc-OSX at https://www.gnome-look.org/content/show.php/Arc-OSX-themes?content=175536.



- autostart must be copied into your ~/GNUstep/Library/Windowmaker directory. You can disable conky, compton or gnome-settings-daemon and the other components by commenting them out.
- compton.conf must be copied into ~/.config/ directory.
- conkyrc must be renamed ~/.conkyrc
- Rik.themed is to be put in  ~/GNUstep/Library/Windowmaker/Themes. You will be able to select it with Windowmaker desktop menu.
- GnomeRikIcons-master is to be put in /usr/share/icons or in ~/local/share/icons
- myDF-Arc-OSX goes to /usr/share/themes or in ~/share/themes.
- you can use Gnome-tweak-tool to use GnomeRikIcons-master and myDF-Arc-OSX in gnome-apps.
- my version of rik.theme for GNUstep can be found at https://github.com/BertrandDekoninck/rik.theme and shall be installed in ~/GNUstep/Library/Themes or in your system GNUstep/Library/Themes folder.
- GWorkspace can be found here : https://github.com/gnustep/apps-gworkspace. I have a slightly modified version here : https://github.com/BertrandDekoninck/gworkspace
- AClock is part of the GNUstep Applications Project and can be found here : https://savannah.nongnu.org/projects/gap
- GSPanel can be found here : https://github.com/BertrandDekoninck/GSPanel.

