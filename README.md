Evil Status Icon Forever
========================

This is a GNOME 3.2 shell extensions that let users have good old applet-like notification area on the top bar.

How to Install
--------------

 1. Clone the code

        cd /home/brianhsu/.local/share/gnome-shell/extensions/
        git clone git://github.com/brianhsu/EvilStatusIconForever.git "EvilStatusIconForever@bone.twbbs.org.tw"

 2. Enable it using gnome-tweak-tool

How to Use
-----------

After install and enable this extension, you should have a file under `~/.local/share/gnome-shell/extensions/EvilStatusIconForever@bone.twbbs.org.tw/extension.js`.

Open this file using your favorite text editor, you should have seen the following code section, just add the application into ``notification`` array to make its notification show on top bar.

You may use `removeStatusIcon` array to control which built-in icon should be hidden.

NOTE!! You have to restart GNOME to make it work after install and change settings!!

    /*****************************************************
     * Statuc Icon Settings
     ****************************************************/
    
    //
    // Add application you want it shows thier notification status
    // icon on top bar to the following list.
    //
    // You may use top/htop to find out the name of application.
    //
    
    var notification = [
        'deadbeef',
        'pidgin',
        'gcin',
    ]

    // The following list will control which bulit-in status
    // icon show be hidden.
    
    var removeStatusIcon = [
        'a11y',         // Accessibility
        // 'volume',
        // 'battery',
        // 'keyboard',
        // 'bluetooth',
        // 'network'
    ]
   
