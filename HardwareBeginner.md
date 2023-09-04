# **PART 2**

This is the second step in the process towards automation!

### **Attention: If you do not have a Windows computer...**

Due to lack of developer, our support of Mac and Linux is limited.
While you can set these programs up on Mac and Linux, you will need to know how to run command-line build scripts.

If you are not willing to do that or you have no idea what this means, then stop. Unfortunately you will not be able to run these programs.

# (1) Select how far into automation you want to get

**No matter the level of automation you need, start here!**

Select your level of automation 

| Microcontroller Only | Computer Controlled |
| --- | --- |
| Basic SwSh Den hosting | All microcontroller programs plus... | 
| SwSh Day Skipping | Automated Dynamax Adventures! |
| SwSh Egg Hatchers | Den Hosting with stats!  |
| Unattended SwSh Shiny Hunts | Autonomous SwSh & BDSP Shiny Hunts! |
| And more... | And more... |

> **WARNING:** **Swich Lite** does *not* output video and thus programs requiring video feedback programs will *not* work.
If you only have a Switch Lite, consider checking our program list (microcontroller-only[^1] and computer-controlled[^2]) to know what you want to use prior to purchase of the hardware.

# (2) Basic Automation Hardware

_Buy the following items below._

1. [Arduino Leonardo Board](https://www.amazon.com/gp/product/B0786LJQ8K)

<img src="https://raw.githubusercontent.com/PokemonAutomation/Microcontroller/master/Wiki/Hardware/images/leonardo.jpg" height="400">

If it doesn't come with the cable, you will need it separately. It is a Micro-USB male to USB-A cable.

**Switch Lite users will also need:**

2. A USB hub or portable dock. ([example](https://www.amazon.com/gp/product/B07JK9DFKH))

> The Switch Lite does not have a USB-A port. Therefore you need either an adapter or a hub to connect the ProMicro. A charging hub or dock is required to simultaneously charge and use the ProMicro.
> 
> Portable docks will work for the Switch Lite, but will not be able to output video over the HDMI.

**Verify you have the following**

1. An Arduino **Leonardo** (from step (2)A)
2. A USB hub or portable dock (if you have a Switch Lite!)

## **If you are only doing Microcontroller Automation proceed to the next step [here](https://github.com/PokemonAutomation/Microcontroller/blob/master/Wiki/Software/Beginner-Windows-ArduinoLeonardo.md)**.
If you are doing Computer Controlled automation, proceed below to buy more hardware.

---

# (3) Additional Hardware for Computer Control Automation

_Buy the necessary items from A, B, C, & D._

**A.** [Adafruit UART](https://www.adafruit.com/product/954)
>    * ***DO NOT get the Prolific (PLxxxx) controllers.* They are cheap, do not work, and they are explicitly blocked in the program.** If you buy outside of this link, verify it is not a PLxxxx. If you buy it anyway, you will be wasting your time and money.**YOU HAVE BEEN WARNED!**
> <img src="https://github.com/PokemonAutomation/ComputerControl/blob/master/Wiki/Hardware/images/uart-adafruit.jpg" height="200">

**B.** [Male-Male Jumper Wires](https://www.amazon.com/dp/B07S1NGQR1)
> * Note: If purchasing the items from this list, you will need Male to Male Jumper wires. The following link is a search for that [type of item](https://www.amazon.com/jumper-wires-male/s?k=jumper+wires+male+to+male)
> **WARNING:** If the link is broken, please notify us in our Discord!
> 
> **WARNING:** If you do ***not*** buy Hardware from this list, you will need to evaluate what you purchased for the correct type of Jumper Wire.
> <img src="https://github.com/PokemonAutomation/ComputerControl/blob/master/Wiki/Hardware/images/jumper-cables.jpg" height="200">

**C.** Purchase a Video capture card ([example](https://www.amazon.com/gp/product/B088HBRM7T))
> * Most cheap capture cards work. Higher end-capture cards may cause issues with color detection.
> <img src="https://github.com/PokemonAutomation/ComputerControl/blob/master/Wiki/Hardware/images/capture-card-nopt.jpg" height="200">

**D.** HDMI Cables (if you don't own any)
> ***Important:** You will need a fairly powerful computer to handle serial programs with video feedback. For a single Switch with video feedback, we recommend a quad core computer no older than 2015. If you want to run 4 Switches all with feedback, we recommend a modern 8-core computer. The computer must also be running 64-bit Windows, though plan to extend support to other operating systems in the future.*
> 
> There are many ways to set this up with varying cost and difficulty. Here we will present some simple options that do not require soldering. If you are experienced with electronics, feel free to do your own thing.

## **If you are doing Computer Controlled automation proceed to the next step [here](https://github.com/PokemonAutomation/Microcontroller/blob/master/Wiki/Software/Beginner-Windows-ArduinoLeonardo.md)**.

---

[^1]: https://github.com/PokemonAutomation/Microcontroller
[^2]: https://github.com/PokemonAutomation/ComputerControl
