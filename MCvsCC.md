# Microcontroller vs Computer controlled programs

First, choose whether you want microcontroller-only programs or computer-controlled ones.

**Microcontroller-only programs:**
- [Full microcontroller-only program list](https://github.com/PokemonAutomation/Microcontroller/blob/master/Wiki/Programs/README.md).
- Supports Pokémon Sword/Shield, Brilliant Diamond/Shining Pearl, Scarlet/Violet.
- Supports any Switch, including Switch Lite.
- Requires one computer (Windows, macOS or Linux), one microcontroller, USB cable and Switch dock.
- Blindly sends button presses
- Less programs available. 
- Programs run less reliably.

**Computer-controlled programs:**
- [Full computer-controlled program list](https://github.com/PokemonAutomation/ComputerControl/blob/master/Wiki/Programs/README.md).
- Supports Pokémon Sword/Shield, Brilliant Diamond/Shining Pearl, Legends Arceus, Scarlet/Violet.
- Most don't support Switch Lite.
- Requires one computer (Windows, macOS or Linux), one microcontroller, Switch dock, capture card and more cables.
- Takes in video input, so it can make decisions based on what’s on screen.
- More programs available. Most new development done on computer control.
- Programs run more reliably.

Microcontroller-only programs function the same as a controller script/programmable game controller.
They send a pre-determined sequence of button presses to Switch.
Whenever you want to run a new program, you need to use dedicated software to build the program file (.hex file) and flash (aka install) it onto the microcontroller.
Then the microcontroller runs the program.
Mac and Linux users need to be a bit computer-savvy and are willing to debug shell scripts to flash microcontroller-only programs.

As the Pokémon game developer Game Freak embraces open world game design, it is more difficult to write reliable microcontroller programs for them. Most of our developers are now focused on computer-controlled programs. There will likely be fewer microcontroller-only programs for future games than for Sword/Shield.

Computer-controlled programs run on your PC. They send button presses to the microcontroller, which relays them to Switch.
Computer-controlled programs can read Switch video stream using a video capture card.
This makes them more powerful than microcontroller-only programs.
Unfortunately, most computer-controlled programs **don't work** with Switch Lite because it does not output video stream.
Check [the program list](https://github.com/PokemonAutomation/ComputerControl/blob/master/Wiki/Programs/README.md)
for which computer-controlled programs work with Switch Lite.  

Computer-controlled programs may be unoptimized on macOS and Linux. A higher-end macOS or Linux machine may be needed.