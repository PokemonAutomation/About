# Tutorial - Mac - All Microcontrollers

This section will walk you through the entire process of setting up your microcontroller on a Mac computer.

For Linux, you will need to find on your own the `apt-get` commands corresponding to the macOS package installation commands listed below.
But since you are using Linux, I would assume you are computer-savy and know how to do this!

At this time, the HexGenerator program used for micro-controller programs on Windows is not yet available for Mac or Linux.
You will need to run and debug a script that is no longer supported by us to generate it.

## Step 1: Acquire the Hardware

Make sure you have one of the hardware:
- [Hardware - Arduino Leonardo](../Hardware/ArduinoLeonardo.md)
- [Hardware - Teensy 2.0 and Teensy++ 2.0](../Hardware/Teensy2.md)
- [Hardware - Pro Micro](../Hardware/ProMicro.md)
- [Hardware - Arduino Uno R3](../Hardware/ArduinoUnoR3.md)

## Step 2: Install Homebrew and AVR

1. Install homebrew: https://brew.sh/
2. Install AVR:
    1. Run `brew tap osx-cross/avr`.
    2. Run `brew install avr-gcc`.
    3. Run `brew install avrdude`.
3. Install fzf: `brew install fzf`

## Step 3: Download the Arduino Programs

Download the latest version of our Arduino programs from [here](https://github.com/PokemonAutomation/Microcontroller/releases).

(The link should look like something like `PASwShNativePrograms-yyyymmdd.zip`)

If you get a virus or malware warning, ignore it. These are known false positives. If you don't trust us, the source code is in this repo.

Once you have downloaded the package, unzip to somewhere you can access later.

## Step 4: Configure the microcontroller program

This step isn't needed for the TurboA example here, but is for nearly every other program.

1. Navigate into the `NativePrograms/NintendoSwitch` folder.
2. Open `TurboA` with a text editor.
> We recommend starting with "Turbo A"  as it is the simplest program. If you are able to get this running, it is easier to troubleshoot the other programs.

Normally you will see a bunch of options that can configured. But TurboA has nothing.

3. After you have made your changes, save the file.

See the documentation for the respective program for a description of all the options.

## Step 5: Build .hex file and flash to the microcontroller

Choose the instructions based on the microcontroller you have:

### For Arduino Leonardo, Pro Micro and Arduino Uno R3:

1. Open Terminal.
2. Type `bash ` (with a trailing space!) Do not hit enter after entering this.
3. Drag from finder the "00-FlashUnix.sh" script in `NativePrograms/NintendoSwitch` folder into the Terminal Window.
4. Press enter.

Once you run the script, it will prompt you for:
- The board type. Enter `ArduinoUnoR3` `ArduinoLeonardo` `ProMicro` depending on your board.
- Which program to compile and load. For this tutorial, enter `TurboA`.

It will automatically build the program and flash it to your device.

### For Teensy 2.0 and Teensy++ 2.0:

1. Download [Teensy Loader](https://www.pjrc.com/teensy/loader_mac.html) if you don't have it yet.

Direct download link: https://www.pjrc.com/teensy/teensy.dmg

2. Open Terminal.
3. Type `bash ` (with a trailing space!) Do not hit enter after entering this.
4. Drag from finder the "00-BuildAllUnix.sh" script in `NativePrograms/NintendoSwitch` folder into the Terminal Window.
5. Press enter.

This will build every single program in the package. As of this writing, there is no easy method to build that is more targeted. If you are confortable with makefiles and command lines, you can directly use the makefile.

6. Run the Teensy Loader program that you downloaded earlier.
7. Click the purple file icon and browse for the .hex that was created in the previous step.

<img src="images/tutorial-windows-teensy-2.png">

8. Plug the Teensy into your computer.
9. Press the white button on the Teensy. You may need to wait for Windows to install drivers.

At this point, two green arrows should show up in Teensy Loader.

<img src="images/tutorial-windows-teensy-3.png">

10. Click the left arrow. This flashes the program into the Teensy.

<img src="images/tutorial-windows-teensy-4.png">

11. Unplug the Teensy from your computer.

## Step 6: Setup and run the program!

1. On your Switch, enter the game and navigate to somewhere you want to mash A in front of (such as the digging duo in Sword/Shield).

<img src="images/digging-duo.jpg" height="400">

2. Navigate to the grip menu without closing the game. This disconnects all controllers from the Switch so that the microcontroller can take over.

<img src="images/grip-menu.jpg" height="400">

3. Plug the microcontroller into your Switch (or the dock that's attached to it).

The program should now begin running. It will flash its light for a few seconds, then it will connect to the Switch and navigate its way back into the game. After a brief pause, it will start mashing A.

**Usage Notes:**

- To stop the program, simply unplug the microcontroller at any time.
- Do not change video output or mess with the HDMI. These can cause the program to Switch to freeze for multiple seconds and break the program. If you want turn off the TV, do it *before* you start the program.

## Other Microcontroller-Only Programs

You now know how to run TurboA - the most basic of the microcontroller-only programs.
You can choose any of the other microcontroller-only programs stored in `NativePrograms` folder and repeat steps 4-6.

- [Program List](https://github.com/PokemonAutomation/Microcontroller/blob/master/Wiki/Programs/README.md)

It is important to read the manual for a program before you use it. Each program has a different set of instructions and startup conditions.

## Computer-Controlled Programs

Now that you are done with the Microncontroller tutorial, you can proceed to the [Computer-Control tutorial](https://github.com/PokemonAutomation/ComputerControl/tree/master/Wiki/Hardware/README.md).

<hr>

**Discord Server:** 

[<img src="https://canary.discordapp.com/api/guilds/695809740428673034/widget.png?style=banner2">](https://discord.gg/cQ4gWxN)


