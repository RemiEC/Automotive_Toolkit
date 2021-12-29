# First thing to do

Please run the bash file in order to delete the unwanted files

# Add new folder into applications menu

Put all the desktop files in /usr/share/backbox/applications   
Put all the directory files in /usr/share/backbox/desktop-directories  
  
In order to add a folder containing some applications, you also have to modify the /etc/xdg/xdg-backbox/menus/xfce-applications.menu :
* Add a line in the "Layout" part like "<Menuname>BackBox-Pentest</Menuname>"
* Add a paragraph like the following, careful to put the right .directoy file and for the category I advise to put the same as the .directory file name :
```xml
<Menu>
    <Name>BackBox-Pentest</Name>
    <Directory>BackBox-Pentest.directory</Directory>
    <Include>
        <Category>BackBox-Pentest</Category>
    </Include>
    <Layout>
        <Merge type="menus"/>
        <Merge type="files"/>
    </Layout>
</Menu>
```

* Finally, you can open the menu editor and put the newly folder wherever you want. You should initially find it at the bottom. Without this step, you won't be able to see your folder in the menu. 

# Add application into a folder

In the .desktop file of the app, match the category with the one you put into the xml above (= the .directoy file name).  
The exec part of the .desktop file should allow you to launch the tool or at least open the terminal with the help command of the tool (ex : "toolname -h")
