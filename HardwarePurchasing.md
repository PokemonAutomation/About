This is the first step in the process towards automation!

# (1) Select how far into automation you want to get

Select your level of automation 

| Microcontroller | Computer Controlled | Auto Max Lair |
| --- | --- | --- |
| Basic Den hosting | All microcontroller programs plus... | Automated Dynamax Adventures!
| Day Skipping | Automated purple beam finder | All Microcontroller programs |
| Egg Hatchers | Den Hosting with stats!  | All Computer Controlled programs |
| Unattended Shiny Hunts | Autonomous Shiny Hunts! |      |

*The levels of automation build off each other, to do Auto Max Lair you have to proceed trhough Microcontroller and Computer Controlled tutorials. You have been warned.*

# (2) Microcontroller Hardware

### A. Buy hardware under the column of what type of Switch you have.

| Switch | Switch Lite |
| --- | --- |
| Mini-USB male to USB-A male cable or adapter. ([example 0](https://www.amazon.com/Cmple-Pack-Male-5-Pin-Adapter/dp/B00A1PH0ZW), [example 1](https://www.amazon.com/gp/product/B00P0GI68M)) | Mini-USB male to USB-A male cable or adapter. ([example](https://www.amazon.com/gp/product/B07QJTX59H/)) |
|     | A USB hub or portable dock. ([example](https://www.amazon.com/gp/product/B07JK9DFKH)) |

Switch Lite notes:
   > The Switch Lite does not have a USB-A port. Therefore you need either an adapter or a hub to connect the Teensy. A charging hub or dock is required to simultaneously charge and use the Teensy.
   > 
   > Portable docks will work for the Switch Lite, but it will not be able to output video over the HDMI.

### B. Buy *one* of the following Microcontrollers.

Select which column best exemplifies your experience and purchase that microcontroller.

| [Teensy](https://www.pjrc.com/store/teensy.html) | [ProMicro](https://www.amazon.com/gp/product/B08BJNV1J3) |
| --- | --- |
| For beginners | Experienced users |
| I want to easily add programs| I want to automate multiple switches, cheaply |
| I'm not experienced with electronics | I know my way around electronics |

### C. Verify you have the following

1. A Mini-USB male to USB-A male cable or adaptor (from step (2)A)
2. A microcontroller (from step (2)2B)
3. A USB hub or portable dock (if you have a Switch Lite!)

**If you are only doing Microcontroller Automation proceed to the next step [here](dead)**
If you are doing Computer Controlled or Auto Max Lair automation, proceed below.

# (3) Additional Computer Controlled Hardware

### A. Serial UART board

Purchase *one* of the following serial boards

| Adafruit UART  | CP210x Board | 
| --- | --- |
| [CP210x controller](https://www.adafruit.com/product/954) | [4 for $8](https://www.amazon.com/gp/product/B07T1XR9FT) |
|   | [1 for $8](https://www.amazon.com/dp/B072K3Z3TL) |
|   | [2 for $8](https://www.amazon.com/gp/product/B07D6LLX19/) |

### B. Serial Board Connections

Purchase *one* of the following Board Connections

| Mini-Grabbers to Male Jumer Wires | Soldless Hammer Headers | Hammer Headers | 
| --- | --- | --- |
| Easiest option, but hard to find | Fairly easy to install. These must have a buldge on the short side. | Most difficult. Will require soldering. |
| [grabbers](https://www.amazon.com/gp/product/B08M5GNY47) | [solderless](https://www.adafruit.com/product/3662) | [headers](https://www.adafruit.com/product/2822) |

### C. Capture Card

Purchase a Video capture card ([example](https://www.amazon.com/gp/product/B088HBRM7T))

### D. HDMI Cables

Purchase HDMI cable(s) if you don't own any

***Important:** You will need a fairly powerful computer to handle serial programs with video feedback. For a single Switch with video feedback, we recommend a quad core computer no older than 2015. If you want to run 4 Switches all with feedback, we recommend a modern 8-core computer. The computer must also be running 64-bit Windows, though plan to extend support to other operating systems in the future.*

> There are many ways to set this up with varying cost and difficulty. Here we will present some simple options that do not require soldering. If you are experienced with electronics, feel free to do your own thing.

**Whether you are doing Computer Controlled or Auto Max Lair Automation proceed to the next step [here](dead)**