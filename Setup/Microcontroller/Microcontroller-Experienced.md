# **Part 2:** Microcontroller setup - experienced users

If you're reading this page, we assume you are a user that is experienced with microcontrollers.

**First, read the [beginner guide to microcontroller setup](./Microcontroller-Beginner.md) to understand how to flash programs onto the microcontroller.** This page only provides supplementary information to the beginner guide.

## Summary of steps
- Step 0: Acquire the [Hardware](/Setup/HardwareNeeded/HardwareExperienced.md)
- Step 1: Install WinAVR
- Step 2: Download the program to flash the microcontroller: QMK Toolbox or Teensy Loader
- Step 3: Download our Arduino Programs
- Step 4: Generate a .hex file
- Step 5: Flash the .hex onto the microcontroller
- Step 6: Setup and run the program!

Refer to the [Beginner guide](./Microcontroller-Beginner.md) for more details.

Below, we highlight the steps that are different from the beginner guide.

## Step 2: Download the program to flash the microcontroller

### If you have the Arduino Leonardo or Pro Micro

Download [QMK Toolbox](https://github.com/qmk/qmk_toolbox/releases).

Refer to the [Beginner guide](./Microcontroller-Beginner.md) for more details.

### If you have the Teensy 2.0 or Teensy++ 2.0 

Download [Teensy Loader](https://www.pjrc.com/teensy/loader.html).

Direct download link: https://www.pjrc.com/teensy/teensy.exe

## Step 5: Flash the .hex onto the microcontroller.

### If you have the Arduino Leonardo

- refer to the [Beginner guide](./Microcontroller-Beginner.md)

### If you have the Pro Micro

1. Run the QMK Toolbox program that you downloaded earlier.
2. Open the .hex you generated in the previous step.
3. Change the MCU to `atmega32u4`.
4. Check the "Auto-Flash" box.

<img src="images/tutorial-windows-pro-micro-2.png" height="600">

5. Plug the Pro Micro into your computer.
6. Short the GND and RST holes. (use tweezers)

<img src="images/tutorial-windows-pro-micro-3.jpg" height="600">

The QMK program will now flash the program to the Pro Micro and show a bunch of logging.

<img src="images/tutorial-windows-pro-micro-4.png" height="600">

7. Unplug the Pro Micro from your computer.

### If you have the Teensy 2.0 or 2.0++

1. Run the Teensy Loader program that you downloaded earlier.
2. Click the purple file icon and browse for the .hex that was created in the previous step.

<img src="images/tutorial-windows-teensy-2.png">

3. Plug the Teensy into your computer.
4. Press the white button on the Teensy. You may need to wait for Windows to install drivers.

At this point, two green arrows should show up in Teensy Loader.

<img src="images/tutorial-windows-teensy-3.png">

5. Click the left arrow. This flashes the program into the Teensy.

<img src="images/tutorial-windows-teensy-4.png">

6. Unplug the Teensy from your computer.

## If you are only doing Microcontroller Automation, your tutorial ends here!

Congrats! You've learned how to automate!

<hr>

## If you are doing Computer Controlled Automation, your next step is [here](/Setup/ComputerControl/ComputerControl-Experienced.md)

The next step will teach you how to put together and use the Computer Controlled hardware.

<hr>

**Discord Server:** 

[<img src="https://canary.discordapp.com/api/guilds/695809740428673034/widget.png?style=banner2">](https://discord.gg/cQ4gWxN)



