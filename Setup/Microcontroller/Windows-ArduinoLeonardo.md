# Windows Tutorial - Arduino Leonardo

This section will walk you through the entire process of setting up your Leonardo on a Windows computer.



## Step 1: Acquire the Hardware

Make sure you have the hardware:

- [Hardware - Arduino Leonardo](../Hardware/ArduinoLeonardo.md)

## Step 2: Install WinAVR

Download and install [WinAVR](https://sourceforge.net/projects/winavr/files/).

It is strongly recommended to install it in the default directory (`C:/WinAVR-20100110`).

## Step 3: Download QMK Toolbox

Download [QMK Toolbox](https://github.com/qmk/qmk_toolbox/releases).

You want the file `qmk_toolbox.exe`.

## Step 4: Download the Arduino Programs

Download the latest version of our Arduino programs from [here](https://github.com/PokemonAutomation/Microcontroller/releases).

(The link should look like something like `PA-NativePrograms-0.x.x-xxxxxxxx.zip`)

If you get a virus or malware warning, ignore it. These are known false positives. If you don't trust us, the [source code is here](https://github.com/PokemonAutomation/Arduino-Source/tree/main/HexGenerator).

Once you have downloaded the package, unzip to somewhere you can access later. Do not put it on Microsoft OneDrive.

## Step 5: Generate a .hex file.

1. Open the package from previous section and double-click on `HexGenerator-Windows.cmd` to run it.
2. In the "Board Type" drop-down, change it to "Arduino Leonardo" depending on which board you have.
3. In the program list, click on "Turbo A".
> We recommend starting with "Turbo A"  as it is the simplest program. If you are able to get this running, it is easier to troubleshoot the other programs.

<img src="images/tutorial-windows-leonardo-0.png">

4. Click on "Save and generate .hex file!".

After a while, you should get a confirmation box saying it was successful. You should now see a file `TurboA-ArduinoLeonardo.hex` in the folder of the programs.

<img src="images/tutorial-windows-leonardo-1.png">

## Step 6: Flash the .hex into the Leonardo.

1. Run the QMK Toolbox program that you downloaded earlier.
2. Open the .hex you generated in the previous step.
3. Change the MCU to `atmega32u4`.
4. Check the "Auto-Flash" box.

<img src="images/tutorial-windows-leonardo-2.png" height="600">

5. Plug the Leonardo into your computer. Wait for the drivers to install.
6. Press the reset button.

<img src="images/tutorial-windows-leonardo-3.jpg" height="400">

The QMK program will now flash the program to the Leonardo and show a bunch of logging.
Afterwards, the 3 LEDs on the Leonardo should flash in unison for 5 seconds before turning off.

<img src="images/tutorial-windows-leonardo-4.png" height="600">

7. Unplug the Leonardo from your computer.

## Step 7: Setup and run the program!

1. On your Switch, enter the game and navigate to somewhere you want to mash A in front of (such as the digging duo).

<img src="images/digging-duo.jpg" height="400">

2. Navigate to the grip menu without closing the game. This disconnects all controllers from the Switch so that the Leonardo can take over.

<img src="images/grip-menu.jpg" height="400">

3. Plug the Pro Micro into your Switch (or the dock that's attached to it).

The program should now begin running. It will flash its lights for a few seconds, then it will connect to the Switch and navigate its way back into the game. After a brief pause, it will start mashing A.

**Usage Notes:**

- To stop the program, simply unplug the Pro Micro at any time.
- Do not change video output or mess with the HDMI. These can cause the program to Switch to freeze for multiple seconds and break the program. If you want turn off the TV, do it *before* you start the program.

## Other Programs

You now know how to run TurboA - the most basic of the programs. You can choose any of the other programs and repeat steps 5-7.

- [Program List](/Wiki/Programs/README.md)

It is important to read the manual for a program before you use it. Each program has a different set of instructions and startup conditions.
You can find the manual for a program by clicking on the "Online Documentation" link.

## Computer-Controlled Programs

Now that you are done with the Microncontroller tutorial, you can proceed to the [Computer-Control tutorial](https://github.com/PokemonAutomation/ComputerControl/tree/master/Wiki/Hardware/README.md).

<hr>

**Discord Server:** 

[<img src="https://canary.discordapp.com/api/guilds/695809740428673034/widget.png?style=banner2">](https://discord.gg/cQ4gWxN)












