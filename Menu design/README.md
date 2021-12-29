# First thing to do

Please run the bash file in order to delete the unwanted files

# Add new folder into applications menu

Put all the desktop files in /usr/share/backbox/applications   
  except these ones which must be placed in /usr/share/applications
    gnuradio-grc.desktop
Put all the directory files in /usr/share/backbox/desktop-directories  
  
Replace the /etc/xdg/xdg-backbox/menus/xfce-applications.menu by the one provided above.

# Add application into a folder

In the .desktop file of the app, match the category with the one you put into the xml above (= the .directoy file name).  
The exec part of the .desktop file should allow you to launch the tool or at least open the terminal with the help command of the tool (ex : "toolname -h")



