# Information

In this folder, you can find all the files required to customize the application menu. 

# Add new folder into applications menu

Put all the desktop files from the usr_share_backbox in /usr/share/backbox/applications   
Put all the desktop files from the usr_share_applications in /usr/share/applications 
Put all the directory files in /usr/share/backbox/desktop-directories  
  
Replace the /etc/xdg/xdg-backbox/menus/xfce-applications.menu by the one provided above.

# Add application into a folder

In the .desktop file of the app, match the category with the one you put into the xml above (= the .directoy file name).  
The exec part of the .desktop file should allow you to launch the tool or at least open the terminal with the help command of the tool (ex : "toolname -h")



