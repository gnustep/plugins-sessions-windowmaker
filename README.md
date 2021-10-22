These are configs and scripts to launch a "mac-like" WindowMaker session with GNUstep. GNUstep will use themes like rik.theme, NesedahRik.theme, NarcissusRik.theme, or Sombre.theme, that use a globalmenubar setting, and icons from It uses gnome-settings-daemon/mate-settings-daemon, conky and compton as compositing manager, and a few GNUstep apps : gdomap; gdnc, GWorkspace, AClock and a persistant panel at the top of the screen : TopBar. A Windowmaker theme, a Gnome theme and an icontheme are also provided so that the look will be more coherent with GNUstep's rik.theme and Sombre.theme.

The windowmaker theme Rik.themed is a modifyed version of the Rhaps theme from https://www.opendesktop.org/s/Window-Managers/p/1018322/. 

For Gnome applications, GnomeRikIcons-master is based on GnomeYosemiteIcons-master from https://raw.githubusercontent.com/ActusOS/GnomeYosemiteIcons. These are to be used with gnustep rik.theme. If  you use Sombre.theme, use https://github.com/vinceliuice/WhiteSur-icon-theme and https://github.com/vinceliuice/WhiteSur-gtk-theme.

myDF-Arc-OSX is a modified version of DF-Arc-OSX at https://www.gnome-look.org/content/show.php/Arc-OSX-themes?content=175536. I hacked this theme to address an issue with compton (duplication of shadows). This theme isn't mandatory anymore since I add the correct option in compton.conf to fix this issue.

- autostart must be copied into your ~/GNUstep/Library/Windowmaker directory. Tweak it ! Each time I install a gnustep environment, I find little bugs I left in this scrpt. You can disable conky, compton or gnome-settings-daemon and the other components by commenting them out.

- compton.conf must be copied into ~/.config/ directory.

- conkyrc must be renamed ~/.conkyrc

- Rik.themed and Sombre.themed for WindowMaker are to be put in  ~/GNUstep/Library/Windowmaker/Themes. You will be able to select it with Windowmaker desktop menu.

- gnome themes like GnomeRikIcons-master and whiteSur-gtk-theme are to be put in /usr/share/icons or in ~/local/share/icons. I whiteSur-gtk-theme must be build and installed using the scripts provided in the github repo.

- myDF-Arc-OSX goes to /usr/share/themes or in ~/share/themes. WhiteSur-Icon-Theme can be configured and installed using the scripts provided in the github repo.

- you can use Gnome-tweak-tool (if using gnome-settings-daemon) or Mate preferences (if using mate-settings-daemon) to use GnomeRikIcons-master and myDF-Arc-OSX in gnome-apps. I prefer to use mate-settings-daemon since gnome-settings-daemon let the pointer disappear if it handles it and you need to adjust this particular settings in the dconf databse.

- rik.theme for GNUstep can be found at https://github.com/AlessandroSangiuliano/rik.theme and shall be installed in ~/GNUstep/Library/Themes or in your system GNUstep/Library/Themes folder. You can set it up for all gnustep's apps by typing this in a terminal : 'defaults write NSGlobalDomain GSTheme Rik'.
![newscreen](https://user-images.githubusercontent.com/12986802/138477523-859a58d3-03ac-4a54-84fa-a644ef8ad1c2.png)

- Sombre.theme for GNUstep can found at https://github.com/gnustep/Sombre
![Screenshot](https://user-images.githubusercontent.com/12986802/138485547-5d5947fc-e259-4b46-b7e4-c45ad338ba3c.png)

- GWorkspace can be found here : https://github.com/gnustep/apps-gworkspace.

- AClock is part of the GNUstep Applications Project and can be found here : https://savannah.nongnu.org/projects/gap

- TopBar can be found here : https://github.com/gnustep/TopBar. Its purpose it to have a persistant bar at the top of the screen when non-gnustep's apps have the focus. For now, TopBar is covered by GNUstep menus when a gnustep app has the focus. If you use a compositor (compton), you can enable the transparency of gnustep's menubar when using rik.theme and typing the following command in a terminal : 'defaults write NSGlobalDomain RikMenuBarTransparency 0.0'. But the widgets of TopBar will still be covered and unclickable when a gnustep app has the focus. This is a work-in-progress. I want to reduce the width of gnustep's menubar in order to leave the right side of TopBar clickable.


Lastly, I wrote several app wrappers for non gnustep's apps. You can install them in any applications directory of GNUstep and relaunch GWorkspace. You will have to set the default app for each particular mimetype using GWorkspace tools inspector (use the #3 shortcut when an icon of the mimtype is selected). You can find these wrappers at https://github.com/gnustep/RikIcons/tree/master/AppWrappers.

Have fun with GNUstep !
