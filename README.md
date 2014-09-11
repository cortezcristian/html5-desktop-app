HTML5 Desktop Application
=================

This example demostrates how to port your HTML5 game into a Desktop App Example with node-webkit. Let's assume you already created an HTML5 Game like [Galaxian Canvas Game](https://github.com/straker/galaxian-canvas-game) but you don't want to host it on the web, you want to share it as a desktop application.

First you need to [download node-webkit](https://github.com/rogerwang/node-webkit#downloads)

Second, put your HTML5 Game and create a [package.json file](https://raw.githubusercontent.com/cortezcristian/html5-desktop-app/master/package.json) for your node-webkit application. Once you have all that simply go into the folder and generate a zip.
    
    zip -r game.zip *
    
Once you have the zip you can try running your game by doing

    ~/node-webkit-v0.10.3-linux-x64$ ./nw /var/www/html5-desktop-app/game.zip


This should be the final result:
![Final Result](https://raw.githubusercontent.com/cortezcristian/html5-desktop-app/master/space-shooter.png)

To pack your app in GNU/Linux you can simply run:

    $ cat ./nw /var/www/html5-desktop-app/game.zip > app && chmod +x app 
