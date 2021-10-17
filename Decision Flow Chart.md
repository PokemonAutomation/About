Struggling trying to decide where to start and what to buy? Use this page to aid your decision making process. This page is to be used by following the headlines in order (1, 2, 3).

# (1) What type of Switch do you have?

| [Switch Lite](https://github.com/PokemonAutomation/About/blob/master/Decision%20Flow%20Chart.md#switch-lite) | [Switch](https://github.com/PokemonAutomation/About/blob/master/Decision%20Flow%20Chart.md#switch) |
| --- | --- |


## Switch Lite

1. Mini-USB male to USB-A male cable or adapter. ([example](https://www.amazon.com/gp/product/B07QJTX59H/))
2. A USB hub or portable dock. ([example](https://www.amazon.com/gp/product/B07JK9DFKH))
   > The Switch Lite does not have a USB-A port. Therefore you need either an adapter or a hub to connect the Teensy. A charging hub or dock is required to simultaneously charge and use the Teensy.
   > 
   > Portable docks will work for the Switch Lite, but it will not be able to output video over the HDMI.
3. A Microcontroller
   > [Help me decide](https://github.com/PokemonAutomation/SwSh-Arduino/wiki/Decision-Flow-Chart#2-what-type-of-microcontroller-should-i-get)



## Switch

1. Mini-USB male to USB-A male cable or adapter. ([example 0](https://www.amazon.com/Cmple-Pack-Male-5-Pin-Adapter/dp/B00A1PH0ZW), [example 1](https://www.amazon.com/gp/product/B00P0GI68M))
2. A Microcontroller
   > [Help me decide](https://github.com/PokemonAutomation/SwSh-Arduino/wiki/Decision-Flow-Chart#2-what-type-of-microcontroller-should-i-get)

***

# (2) What type of microcontroller should I get??

Select which column best exemplifies your experience.

| [Teensy](https://github.com/PokemonAutomation/SwSh-Arduino/wiki/Decision-Flow-Chart#teensy) | [ProMicro](https://github.com/PokemonAutomation/SwSh-Arduino/wiki/Decision-Flow-Chart#promicro) |
| --- | --- |
| For beginners | Experienced users |
| I want to easily add programs| I want to automate multiple switches, cheaply |
| I'm not experienced with electronics | I know my way around electronics |

## Teensy

The Teensy is best suited for people with minimal experience with electronics.

Teensy has 2 flavors: 2.0 and 2.0++ (**Choose one**)
   1. [Teensy 2.0](https://www.pjrc.com/store/teensy.html) 
      1. Sufficient for the programs in this project
   2. [Teensy++ 2.0](https://www.pjrc.com/store/teensypp.html) 
      1. More powerful and expensive than the Teensy 2.0

Here is the installation tutorial for the [Teensy](https://github.com/PokemonAutomation/SwSh-Arduino/wiki/Tutorial:-Windows_Teensy). You can review this after you've completed the end of this tutorial.

## ProMicro


This board is significantly harder to use than the Teensy. But is cheap in bulk and is best suited for farms of multiple Switches running PABotBase where they rarely need to be reprogrammed.

Link to buying the [Pro Micro Board](https://www.amazon.com/gp/product/B08BJNV1J3)

Here is the installation tutorial for the [ProMicro](https://github.com/PokemonAutomation/SwSh-Arduino/wiki/Tutorial:-Windows_ProMicro). You can review this after you've completed the end of this tutorial.

***

# (3) Should I do the Basic or Advanced programs?

Select which column best exemplifies your experiences.

| [Basic Programs](https://github.com/PokemonAutomation/SwSh-Arduino/wiki/Programs:-Basic-List) | [Advanced Programs](https://github.com/PokemonAutomation/SwSh-Arduino/wiki/Programs:-Advanced-List) |
| --- | --- |
| **For beginners** | **Experienced users** |
| I am new to microcontrollers | I've used microcontrollers before |
| I haven't used automation programs before | I have experience with automation |

## Basic Programs

Basic programs start things off simply. All that's required is the microcontroller and adapter. Here you can build your knowledge base of how to use the programs before jumping into the Advanced Programs.

Review the list of the [Basic Programs](https://github.com/PokemonAutomation/SwSh-Arduino/wiki/Programs:-Basic-List) for an idea of what you can do.

### **No extra equipment is required! The basic hardware tutorial stops here. Continue [here](https://github.com/PokemonAutomation/SwSh-Arduino/wiki/Basic-Hardware)**

<img src="https://github.com/PokemonAutomation/SwSh-Arduino/blob/master/Documentation/Tutorials/images/basic-setup.jpg" height="600">

## Advanced Programs

Advanced programs take a decent amount of setup and require additional hardware. We recommend people utilize these programs after getting familiar with the Basic Programs. If you are wanting your computer to automatically recognize a shiny, instead of manually calibrating it, this is the setup for you.

Here is a list of the [Advanced Programs](https://github.com/PokemonAutomation/SwSh-Arduino/wiki/Programs:-Advanced-List) for an idea of what you can do.

<img src="https://github.com/PokemonAutomation/SwSh-Arduino/blob/master/Documentation/Tutorials/images/serial-setup.jpg" height="600">

**Buy the following additional components for Advanced Programs**
1. Serial Board (**Pick one**)
   1. UART Cable ([CP210x controller](https://www.adafruit.com/product/954))
      > ***Avoid the Prolific (PLxxxx) controllers. Many of them are knock-offs that do not work.***
      >  The Adafruit UART cable is reliable and beginner-friendly, but it is also quite expensive.
   2. CP210x board ([4 for $8](https://www.amazon.com/gp/product/B07T1XR9FT)) | ([2 for $8](https://www.amazon.com/gp/product/B07D6LLX19/)) | ([1 for $8](https://www.amazon.com/dp/B072K3Z3TL))
      >  If you are experienced (or confident), these are some cheaper alternatives which also work. These may require a trivial amount of extra wiring.
2. Board Connection (**Pick one**)
   1. Mini-Grabber to Male jumper wires ([example](https://www.amazon.com/gp/product/B08M5GNY47))
       > Easiest option, but item is hard to find
   2. Solderless Hammer Headers ([example](https://www.adafruit.com/product/3662))
       > Fairly easy to install. Ensure you are getting _hammer headers_, they will have a bulge on the short side to hold the pins in place
   3. Hammer Headers ([example](https://www.adafruit.com/product/2822))
       > Most difficult option! You will **need** to solder with this option. Please only pick it if you are comfortable soldering.
3. Video capture card ([example](https://www.amazon.com/gp/product/B088HBRM7T))
4. HDMI cable(s)

***Important:** You will need a fairly powerful computer to handle serial programs with video feedback. For a single Switch with video feedback, we recommend a quad core computer no older than 2015. If you want to run 4 Switches all with feedback, we recommend a modern 8-core computer. The computer must also be running 64-bit Windows, though plan to extend support to other operating systems in the future.*

> There are many ways to set this up with varying cost and difficulty. Here we will present some simple options that do not require soldering. If you are experienced with electronics, feel free to do your own thing.

### **You've got all the parts! The advanced hardware tutorial stops here. Continue [here](https://github.com/PokemonAutomation/SwSh-Arduino/wiki/Advanced-Hardware)**
