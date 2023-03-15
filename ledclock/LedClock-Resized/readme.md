# LedClock-Resized

## About

As its name tells, this is a resized and an easier to make version of ledclock project.

Main differences are:

- all PCBs are under 100mm height so you can order them for like $5 + shipping from [PCBWay.com](https://www.pcbway.com/) .
You can order them directly from [my PCBWay profile](https://www.pcbway.com/project/member/?bmbno=1D9FACD8-0C52-4C) you can download the gerber files and send them to your manufacturer. 
- 3D printed parts can be printed on smaller printers because the base is split in half (you have to assemble it with some M3 screws and nuts). I printed my parts on an Ender3 V2, so I guess anyone can print them.
- 3D printed parts can be printed without supports. Please check 3mf folder to see orientation if you can't figure it out.
- controller board, led 7segments and dots now uses only 0805 SMD components for easier soldering. I don't have a reflow hot-plate so I made the assembly by hand.
- controller board now uses an **ESP32 D1 Mini** [link for reference](https://www.aliexpress.com/item/1005003746817278.html) for more convenience. By using an embedded ESP32 you will have to overcomplicate the board. Another reason for using a dedicated ESP32 D1 Mini was because some of the components required in the original design are impossible to solder by hand (CP2102). Just upload the firmware on the ESP32 Mini (you can use [this awesome tool](https://imeszaros.github.io/ledclock/) for initial flash) and then plug it into the main controller board. Use [this guide](https://github.com/imeszaros/ledclock/blob/master/ledclock/users-guide.md) if you're not familiarized with WLED App 

## Assembly

Assembly of this project is pretty straightforward: 
- order the PCBs and solder them

![28373dad-76af-430c-a674-46bc3df38653](https://user-images.githubusercontent.com/33284097/225260832-e014ee05-3100-40c5-8c8a-fdfabf3fa48a.jpg)

- print the 3D required parts and assemble them (use 4 x M3x20mm screws and nuts to join the base)

![IMG_3756s](https://user-images.githubusercontent.com/33284097/225260905-eb07e417-62f4-4fcd-8a7b-c8a6aaa48eae.jpg)

- flash the firmware on the ESP32 Mini and then connect it to the controller board 

![IMG_4004s](https://user-images.githubusercontent.com/33284097/225225687-42c8acf4-887e-4b77-9996-423cc3cb9869.jpg)

- join the PCBs with the 3D printed parts

![d932719f-d477-4b1a-8fd8-3f6773710fba](https://user-images.githubusercontent.com/33284097/225263167-3286ab95-2398-4f4f-985e-f0eda899dea5.jpg)

**Provide 5V 2A power supply with barrel jack connector.** 
Make your settings in the WLED APP.

## ENJOY !

![34732020s](https://user-images.githubusercontent.com/33284097/225227034-317f5321-3a94-4aa8-82e6-43c88644d651.jpg)



