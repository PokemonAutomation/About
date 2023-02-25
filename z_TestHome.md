# The Home Page
Welcome to the Home Page of setting up your Pokemon automation. 

First order of business is understanding how far into automation you will need to go for what you want to do. The chart below is a simplification of what setup to choose based on the game. The automation level is set by what the majority of types of programs any given game has.

| Game | Automation Level |
| --- | --- |
| Scarlet & Violet | Computer Controlled | 
| Legends of Arceus | Computer Controlled |
| Brilliant Diamond & Shining Pearl | Computer Controlled |
| Sword & Shield | Microcontroller |
| Sowrd & Shield DLC | Computer Controlled |

> For a full list of programs go here for [Microcontroller](https://github.com/PokemonAutomation/Microcontroller/blob/master/Wiki/Programs/README.md) and here for [Computer Controlled](https://github.com/PokemonAutomation/ComputerControl/tree/master/Wiki/Programs).
  
<!-- Thoughts on this table? -->

**Please pay attention to the Step # so that we can better assist you. Ex: 1.A**

---
# [Step 1] Buy Hardware

No matter the level of automation you need, start here!

> _Buy the necessary items from 1.A & 1.B_

## Microcontroller (MC) Hardware Options

###  Step 1.A - Buy hardware under the column of what type of Switch you have.

> | Switch | Switch Lite |
> | --- | --- |
> | Mini-USB male to USB-A male cable or adapter. ([example 0](https://www.amazon.com/Cmple-Pack-Male-5-Pin-Adapter/dp/B084RN3Z3S?th=1), [example 1](https://www.amazon.com/gp/product/B00P0GI68M)) | Mini-USB male to USB-A male cable or adapter. ([example](https://www.amazon.com/gp/product/B07QJTX59H/)) |
> |     | A USB hub or portable dock. ([example](https://www.amazon.com/gp/product/B07JK9DFKH)) |

### Step 1.B - Buy *one* of the following Microcontrollers.
> 
> Select which column best exemplifies your experience and purchase that microcontroller.
> 
> | [Arduino Leonardo](https://www.amazon.com/gp/product/B0786LJQ8K) | [Teensy2.0](https://www.pjrc.com/store/teensy.html) / [Teensy2.0++](https://www.pjrc.com/store/teensypp.html) | [Pro Micro](https://www.amazon.com/gp/product/B08BJNV1J3) |
> | --- | --- | --- | 
> | For beginners | For beginners | Experienced users |
> | I am accustomed to Arduino | I want to easily add programs | I want to automate multiple switches, cheaply |
> | I'm not experienced with electronics | I'm not experienced with electronics | I know my way around electronics |

### Step 1.C - Verify you have the following

> 1. A Mini-USB male to USB-A male cable or adapter (from Step 1.A)
> 2. A USB hub or portable dock (from Step 1.A **only** if you have a Switch Lite!)
> 3. A microcontroller (from Step 1.B)

## Computer Controlled (CC) Hardware Options

**IMPORTANT:** Skip these steps if you are only doing the Microcontroller setup.

**Requirements for Computer-Controlled Programs**

If you would like to use computer-controlled programs, make sure you meet all of the following requirements:

1. You have computer running 64-bit Windows or macOS. As of this writing, no other platforms are supported. But if you use Linux, you should be computer-savvy enough to adapt our macOS guide to work for your Linux. 
2. You have a regular Switch (not a Switch Lite) if you want to use most of the computer-controlled programs (i.e. programs requiring video/audio feedback).
3. Be willing to spend an additional $20 - $50 USD for the new hardware.
4. Your computer must be sufficiently powerful:
- If you intend to control **1** Switch: A dual-core processor @ 3 GHz no older than 2015 should be sufficient.
- If you intend to control **2** Switches: A quad-core processor @ 3 GHz no older than 2015 should be sufficient.
- If you intend to control **4** Switches: 6-8 cores minimum.

> There are many ways to set this up with varying cost and difficulty. Here we will present some simple options that do not require soldering. If you are experienced with electronics, feel free to do your own thing.

> _Buy the necessary items from 1.D, 1.E, 1.F, and 1.G._

###  Step 1.D - Purchase *one* of the following serial boards

> | Adafruit UART  | CP210x Board | 
> | --- | --- |
> | Suggested for beginners | Best if you want to automate multiple switches |
> | [CP210x controller](https://www.adafruit.com/product/954) | [1 for $8](https://www.amazon.com/dp/B072K3Z3TL) |
> |   | [2 for $8](https://www.amazon.com/gp/product/B07D6LLX19/) |
> |   | [4 for $8](https://www.amazon.com/gp/product/B07T1XR9FT) |

### Step 1.E  Serial Board Connections

Purchase *one* of the following Board Connections

> | [Mini-Grabbers to Male Jumper Wires](https://www.amazon.com/gp/product/B08M5GNY47) | [Solderless Hammer Headers](https://www.adafruit.com/product/3662) | [Hammer Headers](https://www.adafruit.com/product/2822) | 
> | --- | --- | --- |
> | **Arduinos only need these** | N/A for Arduinos | N/A for Arduinos |
> | Easiest option, but hard to find. | Fairly easy to install. These must have a bulge on the short > side. | Most difficult. Will require soldering. |
> | No soldering. Best for beginners. | Doesn't require soldering. | Requires soldering. Experienced only. |

### Step 1.F  Capture Card

> Purchase a Video capture card ([example](https://www.amazon.com/gp/product/B088HBRM7T))

`Note: More expensive cards like the Elgato HD60S tend to have color correction issues you will need to sort through. In general, cheaper $15 cards tend to work fine.`

### Step 1.G HDMI Cables

> Purchase HDMI cable(s) if you don't own any

# [Step 2] Setup the MC Hardware

Before you begin, make sure **you have a computer.** This used to go without saying, but it's becoming apparent that many people do not have computers anymore and only have phones or tablets. You need to have a Windows, macOS or Linux laptop/desktop computer (or a high-end Windows tablet) that you can install software on it.

> For a Microcontroller setup, you need three things setup as follows:
> 1. The Microcontroller (Leonardo, Teensy, or ProMicro) connected to the...
> 2. USB-mini to USB-A cable connected to...
> 3. Your PC
> 
> **Microcontroller -> USB Cable -> PC**

## [Step 3] How to flash the TurboA `.hex` file

Flashing the `.hex` file type is paramount to utilizing our programs. This is the base-level of what you need to handle for automation.

> 1. Open the package from previous section and double-click on HexGenerator-Windows.cmd to run it.
> In the "Board Type" drop-down, change it to `your purchased Microcontroller`.
> In the program list, click on "Turbo A".


#### [Step 4] Device Specific MC Flash Instructions

Click the link below based on the microcontroller and OS.

> | | Windows | macOS or Linux |
> | --- | --- | --- |
> | Arduino Leonardo (beginner friendly) | [Guide](../Software/Windows-ArduinoLeonardo.md) | [Guide](../Software/Mac.md) |
> | Teensy 2.0 and Teensy++ 2.0 | [Guide](../Software/Windows-Teensy2.md) | [Guide](../Software/Mac.md) |
> | Pro Micro | [Guide](../Software/Windows-ProMicro.md) | [Guide](../Software/Mac.md) |
> | Arduino Uno R3 (not recommended)| [Guide](../Software/Windows-ArduinoUnoR3.md) | [Guide](../Software/Mac.md) |

---
# [Step 5] Setup the CC Hardware
####  Device specific CC setup
# [Step 6] Preparing the Device
# [Step 7] Running the Program
