# LedClock-Resized

As its name tells, this is a resized and an easier to make version of @imeszaros ledclock project.

Main differences are:

- all PCBs are under 100mm height so you can order them for like $5 + shipping from [PCBWay.com](https://www.pcbway.com/) .
You can order them directly from [my PCBWay profile](https://www.pcbway.com/project/member/?bmbno=1D9FACD8-0C52-4C) you can download the gerber files and send them to your manufacturer. 
- 3D printed parts can be printed on smaller printers because the base is split in half (you have to assemble it with some M3 screws and nuts). I printed my parts on an Ender3 V2, so I guess anyone can print them.
- 3D printed parts can be printed without supports. Please check 3mf folder to see orientation if you can't figure it out.
- controller board, led 7segments and dots now uses only 0805 SMD components for easier soldering. I don't have a reflow hot-plate so I made the assembly by hand.
- controller board now uses an ESP32 D1 Mini [link for reference](https://www.aliexpress.com/item/1005003746817278.html) for more convenience. By using an embedded ESP32 you will have to overcomplicate the board. Another reason for using a dedicated ESP32 D1 Mini was because some of the components required in the original design are impossible to solder by hand (CP2102). Just upload the firmware on the ESP32 Mini (you can use [this awesome tool](https://imeszaros.github.io/ledclock/) for initial flash) and then plug it into the main controller board. Use [this guide](https://github.com/imeszaros/ledclock/blob/master/ledclock/users-guide.md) if you're not familiarized with WLED App 

# Pictures

![IMG_4004s](https://user-images.githubusercontent.com/33284097/225225687-42c8acf4-887e-4b77-9996-423cc3cb9869.jpg)

![3473208s](https://user-images.githubusercontent.com/33284097/225227013-b22d08b5-69d1-4579-a398-aab7fb6f7612.JPG)

![34732020s](https://user-images.githubusercontent.com/33284097/225227034-317f5321-3a94-4aa8-82e6-43c88644d651.jpg)

