Configs and scripts to launch a WindowMaker session with GNUstep, gnome-settings-daemon/mate-settings-daemon, conky and compton as compositing manager, and a few GNUstep apps : gdomap; gdnc, GWorkspace, AClock and a persistant panel at the top of the screen : TopBar. A Windowmaker theme, a Gnome theme and an icontheme are also provided so that the look will be more coherent with GNUstep's rik.theme.

The windowmaker theme Rik.themed is a modifyed version of the Rhaps theme from https://www.opendesktop.org/s/Window-Managers/p/1018322/. 

GnomeRikIcons-master is based on GnomeYosemiteIcons-master from https://raw.githubusercontent.com/ActusOS/GnomeYosemiteIcons

myDF-Arc-OSX is a modified version of DF-Arc-OSX at https://www.gnome-look.org/content/show.php/Arc-OSX-themes?content=175536. I hacked this theme to address an issue with compton (duplication of shadows). This theme isn't mandatory anymore since I add the correct option in compton.conf to fix this issue.

- autostart must be copied into your ~/GNUstep/Library/Windowmaker directory. You can disable conky, compton or gnome-settings-daemon and the other components by commenting them out.

- compton.conf must be copied into ~/.config/ directory.

- conkyrc must be renamed ~/.conkyrc

- Rik.themed is to be put in  ~/GNUstep/Library/Windowmaker/Themes. You will be able to select it with Windowmaker desktop menu.

- GnomeRikIcons-master is to be put in /usr/share/icons or in ~/local/share/icons

- myDF-Arc-OSX goes to /usr/share/themes or in ~/share/themes.

- you can use Gnome-tweak-tool (if using gnome-settings-daemon) or Mate preferences (if using mate-settings-daemon) to use GnomeRikIcons-master and myDF-Arc-OSX in gnome-apps. I prefer to use mate-settings-daemon since gnome-settings-daemon let the pointer disappear if it handles it and you need to adjust this particular settings in the dconf databse.

- my version of rik.theme for GNUstep can be found at https://github.com/BertrandDekoninck/rik.theme and shall be installed in ~/GNUstep/Library/Themes or in your system GNUstep/Library/Themes folder. You can set it up for all gnustep's apps by typing this in a terminal : 'defaults write NSGlobalDomain GSTheme Rik'.

- GWorkspace can be found here : https://github.com/gnustep/apps-gworkspace. I have a slightly modified version here : https://github.com/BertrandDekoninck/gworkspace with white labels for icons on the desktop and a singleclick setting for the dock. To enabloe single click, type 'defaults write GWorkspace dockclickpolicy 1'.

- AClock is part of the GNUstep Applications Project and can be found here : https://savannah.nongnu.org/projects/gap

- TopBar can be found here : https://github.com/BertrandDekoninck/TopBar. Its purpose it to have a persistant bar at the top of the screen when non-gnustep's apps have the focus. For now, TopBar is covered by GNUstep menus when a gnustep app has the focus. If you use a compositor (compton), you can enable the transparency of gnustep's menubar when using rik.theme and typing the following command in a terminal : 'defaults write NSGlobalDomain RikMenuBarTransparency 0.0'. But the widgets of TopBar will still be covered and unclickable when a gnustep app has the focus. This is a work-in-progress. I want to reduce the width of gnustep's menubar in order to leave the right side of TopBar clickable.

