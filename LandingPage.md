#  Pokémon Automation (Landing Page)

Welcome to Pokémon Automation's official GitHub group.

[<img src="https://canary.discordapp.com/api/guilds/695809740428673034/widget.png?style=banner2">](https://discord.gg/cQ4gWxN)

## What is this?

Pokémon Automation is a project that strives to automate the Pokémon games.

### Why automate the game?

Certain aspects of Pokémon are very boring and tedious (such as shiny hunting). So rather than spending hundreds of hours grinding with manual gameplay, you have a bot do it for you. Thus the fun changes to managing the bots that play the game for you.

With automation, it becomes possible to play 24/7 and simultaneously on multiple devices without wasting too much of your own time. Thus with so much extra game time, it becomes possible to legitimately obtain extremely rare Pokémon that are normally only feasible via hacking.

### How does this work?

The Nintendo Switch allows the use of 3rd party wired controllers. But instead of using an actual game controller, we use a [microcontroller](https://en.wikipedia.org/wiki/Microcontroller) (small programmable computer chip) such as an Arduino, available and affordable on Amazon. This microcontroller can be programmed to send button presses to the Switch to act as a game controller. Once programmed, all that is needed is to plug the microcontroller into your Switch's USB port just like any handheld controller and watch it do its thing.

This approach is not new. brianuuuSonic's AutoController[(1)](README.md#1-brianuuusonics-autocontroller) was (probably?) the first to do this for Switch-based Pokémon games.

You can take a look at our version of these "microcontroller-only" programs [here](https://github.com/PokemonAutomation/Microcontroller/blob/master/Wiki/Programs/README.md).

<img src="images/basic-setup.jpg" width="400"> <img src="images/ShinyHuntUnattended-Regi-0.png" width="500">


### What do we do differently?

While most automation is entirely Arduino or microcontroller based, we have taken it to a new level. We connect the microcontroller to a PC to utilize the full computing potential of a modern computer. This allows us to perform visual recognition of the display and make gameplay decisions the same way a human player would.

This has allowed us to automate every single shiny hunting method in Pokémon Sword/Shield, including automatic shiny hunting of wild Pokémon, legendary Pokémon in Crown Tundra DLC, and automatic egg program to hatch shiny Pokémon.

We have programs for Pokémon Home, Pokémon Brilliant Diamond/Shining Pearl, Pokémon Legends Arceus and the newest Pokémon Scarlet/Violet as well to automate shiny hunting and other tedious tasks.

These "computer-controlled" programs can be found [here](https://github.com/PokemonAutomation/ComputerControl/blob/master/Wiki/Programs/README.md).

**Examples:**

Automatic detection of shiny encounters using visual recognition of the shiny sparkle animation.
<img src="images/ShinyHuntAutonomous-Overworld-1.png" width="800">

Automatic playthrough of Dynamax Adventures to shiny-hunt legendaries.
<img src="images/MaxLair-0.png" width="800">

Shiny detection in Pokémon Legends Arceus using audio recognition.
<img src="images/PLA-ShinyDetection-0.png" width="800">


## Get Me Started!

Interested? Continue reading!

### 1. Select how far into automation you want to get

First of all, choose whether you need microcontroller-only programs or computer-controlled ones.

**Microcontroller-only programs:**
- Require one computer, one microcontroller, USB cable and Switch dock.
- All microcontroller-only programs work with any Switch, including Switch Lite.
- Function the same as a controller script/programmable game controller: send a pre-determined sequence of button presses to Switch.
- Whenever you want to run a new program, you need to use dedicated software to build the program file (.hex file) and flash (aka install) it ont the microcontroller.
- Mac and Linux users need to be computer-saavy and are willing to debug shell scripts to use most of the microcontroller-only programs.
- Include Sword/Shield programs like basic den hosting, day skipping, egg fetching, egg hatching and unattended shiny hunting. Check our full [microcontroller program list](https://github.com/PokemonAutomation/Microcontroller/blob/master/Wiki/Programs/README.md).
- Due to Pokémon Brilliant Diamond/Shining Pearl being unstable on receiving button presses, we don't have microcontroller programs for it.
- As the Pokémon game developer Game Freak embraces open world game design, it is more difficult to write reliable microcontroller programs for them. We don't yet have microcontroller programs for Pokémon Legends Arceus and Pokémon Scarlet/Violet. Future games are likely to be difficult for microcontroller programs as well.

**Computer-controlled programs:**
- Require one computer, one microcontroller, Switch dock, capture card and more cables.
- Most computer-controlled programs **don't work** with Switch Lite because it does not output video streams. Check our [computer-controlled program list](https://github.com/PokemonAutomation/ComputerControl/blob/master/Wiki/Programs/README.md) for which programs work with Switch Lite.  
- Can use capture card to read video and audio streams to your personal computer to compute the best actions in real time.
- Can use your computer to send commands directly into microcontroller, so you don't need to build and flash a .hex file to microcontroller every time. For example, you can [send a new Scarlet/Violet raid code immediately](https://github.com/PokemonAutomation/ComputerControl/blob/master/Wiki/Programs/PokemonSV/FastCodeEntry.md) to microcontroller to let it type the raid code faster than manual typing. You cannot achieve this by a microcontroller-only program as it will take time to build and flash the .hex file containing the raid code. By then the raid lobby will be full.
- Work with Windows, macOS or Linux computers. Programs on macOS and Linux may be unoptimized. A higher-end macOS or Linux machine may be needed.
- Include all microcontroller programs plus programs using video and audio feedback, like automated Dynamax Adventures in Crown Tundra, fully automated wild shiny hunting in Sword/Shield and BDSP, automated raid den hosting with stats in Sword/Shield and Scarlet/Violet, and fully automated shiny egg hunting in Sword/Shield, Brilliant Diamond/Shining Pearl and Scarlet/Violet. Check our full [computer-controlled program list](https://github.com/PokemonAutomation/ComputerControl/blob/master/Wiki/Programs/README.md).
- Due to the trend of open world gameplay in Pokémon games, computer-controlled programs will be the major focus of our development in future.


### 2. Follow tutorial

After you determine whether you need microcontroller-only or computer-controlled programs,
follow the [tutorial](https://github.com/PokemonAutomation/Microcontroller/blob/master/Wiki/Tutorial/Tutorial.md) to purchase hardware and set up the program.



## Credits

**Contributors:**

- [Kuroneko (Kuroneko#6019)](@Mysticial) - Project founder.
- [Gin (Gin#2531)](@Gin890) - R&D, Program+Framework development, Qt6, audio, and Mac support.
- [pifopi (pifopi#7834)](@pifopi) - R&D, AutoMaxlair, Program+Framework Development.
- [MrDonders (MrDonders#4095)](@ercdndrs) - R&D, AutoMaxlair, pioneer of serial hardware.
- [Koi (Koi#3088)](@Koi-3088) - Discord bot integration.
- [denvoros (denvoros#0001)](@denvoros) - AI R&D, AutoMaxlair, Build scripts, Mac support.
- [SakuraKim (SakuraKim#9422)](@SakuraKimAce) - R&D, Program+Framework Development.
- [Fye (Fye#7349)](@fyex) - Program Development
- [Ryder (_Ryder#0149)](@Ensamma) - Documentation and wiki management.
- [baboul (baboul#7130)](@mb-baboul) - Program Contributor
- [joyrida (JoyRida#6391)](@RickyGrassmuck) - Build scripts and Mac support.
- Ptamalion (Ptamalion#1167) - Program Contributor and Qt6 support.
- [Icaroto (Icaroto#9259)](@Icaroto) - Program Contributor
- b0bness (b0bness#9479) - Program Contributor
- [kichithewolf (kichithewolf#5141)](@kichithewolf) - Program Contributor

And countless users and testers in the Pokémon Automation Discord Server.


## Supporting Us

As of this writing, we do not take donations of any kind for this project. The only support we request is by sharing our work with your friends if you have enjoyed using it.
In the spirit of transparency, we kindly ask that you disclose the use of automation when sharing photos or videos of Pokémon obtained using these programs.
This can be done simply by sharing a screenshot of the program with stats or with a text footer indicating it is done by automation.

If such a disclosure is not permissible, we ask that you avoid any explicit or implicit claims that such Pokémon were caught manually.


## License

You are free to use our software personal use only.

Do not try to profit off of these programs. It's just a game; keep the money out of it and have fun.

For all other uses, please reach out to the administrators of the Pokémon Automation discord server.

This software is provided "as is" and the developers disclaim all warranties with regard to this software including all implied warranties of merchantability and fitness. In no event shall the developers be liable for any special, direct, indirect, or consequential damages, or any damages whatsoever resulting from loss of use, data or profits, whether in an action of contract, negligence or other tortious action, arising out of or in connection with the use or performance of this software.

# References
### (1) [brianuuuSonic's AutoController](https://github.com/brianuuu/AutoController_swsh)
### (2) [Microcontroller Repo](https://github.com/PokemonAutomation/Microcontroller)
### (3) [Computer-Control Repo](https://github.com/PokemonAutomation/ComputerControl) 

