
<p align="center">
  <a href="https://raw.githubusercontent.com/imeszaros/ledclock/master/LICENSE"><img src="https://img.shields.io/github/license/mariusmym/LedClock-Resized?color=blue&style=flat-square"></a>
  <a href="https://github.com/Aircoookie/WLED-App"><img src="https://img.shields.io/badge/app-wled-blue.svg?style=flat-square"></a>
  <a href="https://www.printables.com/model/189433-wi-fi-connected-led-clock-powered-by-wled"><img src="https://img.shields.io/badge/models-printables-orange.svg?style=flat-square"></a>
  <a href="https://imeszaros.github.io/ledclock/"><img src="https://img.shields.io/badge/install-esp%20web%20tools-green"></a>
</p>

# LedClock-Resized

## About

As its name tells, this is a resized and an easier to make/print version of [ledclock project](https://github.com/imeszaros/ledclock). 

There are TWO resized dimensions available: 
  1. 52x92mm digits version : 
  2. 40x66mm digits version : 

Since the project is basically the same (except for digits PCBs and 3D printed parts)i though there's no point to make another fork.

This fork is intended just to share the Gerbers and 3D files I used for this remix. If you need more detailed informations, please read descriptions and assembly guide from the [original repository](https://github.com/imeszaros/ledclock).
[imeszaros](https://github.com/imeszaros) did an oustanding job in providing all the explanations required. 

Main differences are:

- all PCBs are under 100mm height so you can order them for like $5 + shipping from [PCBWay.com](https://www.pcbway.com/) .
You can also order them directly from [my PCBWay profile](https://www.pcbway.com/project/member/?bmbno=1D9FACD8-0C52-4C) you can download the gerber files and send them to your manufacturer. 
- 3D printed parts can be printed on smaller printers because the base is split in half (you have to assemble it with some M3 screws and nuts). I printed my parts on an Ender3 V2, so I guess anyone can print them.
- 3D printed parts can be printed without supports. Please check 3mf folder to see orientation if you can't figure it out.
- controller board, led 7segments and dots now uses only 0805 SMD components for easier soldering. I don't have a reflow hot-plate so I made the assembly by hand.
- controller board now uses an **ESP32 D1 Mini** [link for reference](https://www.aliexpress.com/item/1005003746817278.html) for more convenience. By using an embedded ESP32 you will have to overcomplicate the board. Another reason for using a dedicated ESP32 D1 Mini is because some of the components required in the original design are impossible to solder by hand (CP2102). I
f you want, **you can use the original controller board design**, is fully compatible with **LedClock-Resized**.

## Firmware

Firmware is provided by the awesome work of [imeszaros](https://github.com/imeszaros). 
Just connect the ESP32 Mini onto the computer (be sure you have drivers installed for your board USB-TTL chip) and use [this awesome tool](https://imeszaros.github.io/ledclock/) for initial flash. Then plug the ESP32 it into the main controller board

## Assembly

Assembly of this project is pretty straightforward: 
- order the PCBs and solder them

![28373dad-76af-430c-a674-46bc3df38653](https://user-images.githubusercontent.com/33284097/225260832-e014ee05-3100-40c5-8c8a-fdfabf3fa48a.jpg)

![IMG_3859](https://user-images.githubusercontent.com/33284097/225264999-68a3b3eb-f121-4b17-bbce-71934203925d.jpg)


- print the 3D required parts and assemble them (use 4 x M3x20mm screws and nuts to join the base)

![IMG_3756s](https://user-images.githubusercontent.com/33284097/225260905-eb07e417-62f4-4fcd-8a7b-c8a6aaa48eae.jpg)

![d58b3460-f934-42f0-a672-9b96344d7cfe](https://user-images.githubusercontent.com/33284097/225268872-84bfbeff-a710-4290-a9c6-510880cce183.jpg)


- flash the firmware on the ESP32 Mini and then connect it to the controller board.

![IMG_4004s](https://user-images.githubusercontent.com/33284097/225225687-42c8acf4-887e-4b77-9996-423cc3cb9869.jpg)

- join the PCBs with the 3D printed parts

![d932719f-d477-4b1a-8fd8-3f6773710fba](https://user-images.githubusercontent.com/33284097/225263167-3286ab95-2398-4f4f-985e-f0eda899dea5.jpg)

![IMG_1876s](https://user-images.githubusercontent.com/33284097/225265164-2a76d4e5-60c1-4a1f-b002-5c01b62f5aec.jpg)


- **provide 5V 2A power supply with  2.5mm x 5.85mm barrel jack connector.** 
- make your settings in the WLED APP. Use [this guide](https://github.com/imeszaros/ledclock/blob/master/ledclock/users-guide.md) if you're not familiarized with WLED App.

## ENJOY !

![34732020s](https://user-images.githubusercontent.com/33284097/225227034-317f5321-3a94-4aa8-82e6-43c88644d651.jpg)



