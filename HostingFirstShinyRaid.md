# How to host your first raid

This page is provided as a courteous and may not cover all the questions you have about hosting. We suggest spending some time looking up videos on YouTube if you need a visual explanation in addition to this.

**Related Programs:**
- **DaySkippers:**
   - [DaySkipperUS](https://github.com/PokemonAutomation/Microcontroller/blob/master/Wiki/Programs/PokemonSwSh/DaySkipperUS.md)
   - [DaySkipperEU](https://github.com/PokemonAutomation/Microcontroller/blob/master/Wiki/Programs/PokemonSwSh/DaySkipperEU.md)
   - [DaySkipperJPN](https://github.com/PokemonAutomation/Microcontroller/blob/master/Wiki/Programs/PokemonSwSh/DaySkipperJPN.md)
   - [DaySkipperJPN-7.8k](https://github.com/PokemonAutomation/Microcontroller/blob/master/Wiki/Programs/PokemonSwSh/DaySkipperJPN-7.8k.md)
- **Beam Finding:**
   - [Beam Reset](https://github.com/PokemonAutomation/Microcontroller/blob/master/Wiki/Programs/PokemonSwSh/BeamReset.md)
   - [Purple Beam Finder](https://github.com/PokemonAutomation/ComputerControl/blob/master/Wiki/Programs/PokemonSwSh/PurpleBeamFinder.md)
- **Hosting**
   - [Den Roller](https://github.com/PokemonAutomation/Microcontroller/blob/master/Wiki/Programs/PokemonSwSh/DenRoller.md)
   - [AutoHost Rolling](https://github.com/PokemonAutomation/Microcontroller/blob/master/Wiki/Programs/PokemonSwSh/AutoHost-Rolling.md)

*** 
### Pre-requisites
* **PATIENCE**
* A Switch with Sword or Shield
* Nintendo Online
* Access to a discord server with a seed checking bot (sysbot)
* Some time
* Lots of Wishing Pieces
   > You can run the [Watt Farmer](https://github.com/PokemonAutomation/Microcontroller/blob/master/Wiki/Programs/PokemonSwSh/DateSpam-WattFarmer.md) to easily buy more

### Terminology

Frame: Refers to the locked conditions contained inside of a single day in your game, whether it be the Pokémon in a den, the weather, etc.

Seed: Formally known as the Pokémon ID (PID), this is what determines if a Pokemon is Shiny.

SysBot (seed checker): A Switch with CFW running a program to check our Seed. 

Re-Rolling: Manipulating the frame to change what Pokémon you can raid from the den.

***

## Setup Instructions

1. Start at the home menu, all games closed. 
2. Setup Switch Settings
   * Open switch settings
   * Go to System
   * Then Date and Time
   * Turn off “Sync time via internet”
3. Open the game, turn auto-save off in the setting menu. 
4. Find a den that has a Pokémon you want.

## Securing a den

To start off, we will work through obtaining the correct beam you want and finding out information on the den you want.

1. Approach an empty den
2. Activate the den
   1. If you need a rare den (purple beam): follow [Beam Reset](https://github.com/PokemonAutomation/Microcontroller/blob/master/Wiki/Programs/PokemonSwSh/BeamReset.md) if you have a MC Setup _or_ [Purple Beam Finder](https://github.com/PokemonAutomation/ComputerControl/blob/master/Wiki/Programs/PokemonSwSh/PurpleBeamFinder.md) if you have a CC Setup.
   2. If you need a normal den (red beam) use a wishing piece. There is a 1/10 chance the beam will be purple and you will need to clear the den and try again. Conversely you can use [Beam Reset](https://github.com/PokemonAutomation/Microcontroller/blob/master/Wiki/Programs/PokemonSwSh/BeamReset.md) and manually stop the program when you have a red beam.
3. Your game will save automatically, but do not save it yourself after that point. 
4. Enter the raid, defeat the Pokémon, and catch it. **DO NOT SAVE**
5. Connect to the internet in Y-Comm
6. In a server with a seed-bot: look for the commands it uses and follow suit. (Might be $seed, $seedcheck etc etc.) 
7. The bot will message you a code, match with the bot in a link trade. 
8.  Select the Pokémon you caught from your den and offer it for trade. The bot will cancel the trade automatically, and then DM you with information about the trade including, most importantly, your Seed. 
      1. If you are here from our Discord, the bot will tell you how many frames until your next star and square shiny.
      2. If you want more control over what options you have there are different programs that do that: Leanny, Raidfinder, etc. Since this is an introductory explanation, we won't cover those.
9. Take the number the bot gave you for your next shiny frame and subtract three.
   > EX: Next star shiny frame is 1257 frames away.
   > 
   > 1257 - 3 = 1254 (target number)
   1. You **can** subtract more if you want more room. Adjust your target number as you see fit.
   2. Saving three frames in front of your shiny frame will allow you to re-roll your den. This will be discussed at length later.
10. WITHOUT SAVING: close your game to re-obtain your beam that you had just defeated. 

## Day Skipping

Now you have an idea of how far away your shiny frame is and it is time to day skip.

1. Start your game again, and you should find yourself in front of the den with the beam intact. 
2. Go to a secure indoor location in game like a Pokécenter and save your game. 
   1. The dojo inside Isle of Armor is not reliable
3. Open Y-Comm and connect to Internet. 
4. Select Link battle and attempt to start a singles link battle.
5. When the game backs you out of Y-Comm: Hold the Home Button to access quick settings. 
6. Toggle airplane mode as soon as the text announcing a match was found appears, on and off again to disconnect from the internet.
7. Press the Home button to hide Quick Settings. 
8. Click "B" through the warnings.
9. Click the home button and return to the Home menu.
   1. Re-enter the game. If the screen "blinks", you know the glitch was done correctly.
10. Go to the Date and Time menu in Switch settings
11. Run one of the 4 Day Skippers
      1. [DaySkipperUS](https://github.com/PokemonAutomation/Microcontroller/blob/master/Wiki/Programs/PokemonSwSh/DaySkipperUS.md)
      2. [DaySkipperEU](https://github.com/PokemonAutomation/Microcontroller/blob/master/Wiki/Programs/PokemonSwSh/DaySkipperEU.md)
      3. [DaySkipperJPN](https://github.com/PokemonAutomation/Microcontroller/blob/master/Wiki/Programs/PokemonSwSh/DaySkipperJPN.md)
      4. [DaySkipperJPN-7.8k](https://github.com/PokemonAutomation/Microcontroller/blob/master/Wiki/Programs/PokemonSwSh/DaySkipperJPN-7.8k.md)
      > You can change your Switch settings to be in Japanese to utilize the JPN Day Skipper.
      > Follow the instructions on those pages for correct setup and use.
12. Wait for the DaySkipper to finish.
13. Return to the game and **save**.

## Verify distance to shiny frame 

At this point, you are 3 (or more) frames away from your shiny frame. You will need to verify the Day Skipper didn't drop any skips.

1. Collect watts from the den.
2. Save.
3. Enter the den and capture the Pokémon. **DO NOT SAVE**
4. Seedcheck the Pokémon you caught.
   1. Follow prior instructions if you need a refresher.
   2. Verify the number of days away from the shiny frame. If you did it correctly, it will be 3 (or however far away you set it to) frames away.
5. WITHOUT SAVING, close your game to re-obtain your beam that you had just defeated.

   > For reference, Frame 4 is always the shiny frame but it is found after three skips. it goes:
   > 
   > Frame 1 => skip => Frame 2 => skip => Frame 3 => skip => Frame 4

## Check for Shininess

After verifying how far you are from your shiny frame, you double check the den actually has a shiny.

1. Use the [Den Roller](https://github.com/PokemonAutomation/Microcontroller/blob/master/Wiki/Programs/PokemonSwSh/DenRoller.md) to roll to your shiny frame 3 (or more) frames away.
   1. Follow the instruction on the page for correct setup and use.
2. When the program whistles at you, stop the program.
   1. MC users:
      1. _Turn your TV sound on_
      2. This means removing the device from the dock.
   2. For CC users:
      1. Follow the Serial Guide to [Setup Sound](https://github.com/PokemonAutomation/ComputerControl/blob/master/Wiki/Software/Windows.md#step-7-setup-sound).
      2. you can stop the program.
3. Enter the raid.
4. Verify the Pokémon is shiny
   1. If it isn't, go back to seed checking and work your way back here.
5. WITHOUT SAVING, close your game to re-obtain the raid beam.

## Hosting!

You've done everything to get to the shiny frame. Now is the big moment where you decide what to host (soft or hard lock) and how you host.

1. Decide how you plan on hosting:
   1. For hosting a hard-lock (only hosts 1 Pokémon): [Go here](https://github.com/PokemonAutomation/About/blob/master/HostingFirstShinyRaid.md#hard-lock-hosting)
   2. For hosting a soft-lock (hosts the *whole den): [Go here](https://github.com/PokemonAutomation/About/blob/master/HostingFirstShinyRaid.md#soft-lock-hosting)
      * *Dependent on number of badges you have. 1-3 badges can only host 1-2 star shiny raids. Having all 8 badges allows you to hose 3-5 star shiny raids.

## Hard-lock Hosting

This method is if you only want to host _one_ of the Pokémon in the den (ex: G-max Charizard).

1. Open your game and collect watts from the den (if not collected already).
2. Use [Den Roller](https://github.com/PokemonAutomation/Microcontroller/blob/master/Wiki/Programs/PokemonSwSh/DenRoller.md) to roll to your shiny frame.
   > Watch the program so you can stop it when it finds the Pokémon you want!
3. Once you have rolled to the shiny frame _and_ found the Pokémon you want: **SAVE**
4. Use [AutoHost Rolling](https://github.com/PokemonAutomation/Microcontroller/blob/master/Wiki/Programs/PokemonSwSh/AutoHost-Rolling.md) to host!
   > Follow the instruction on the page for correct setup and use.

## Soft-lock Hosting

This method is if you want to host the entire den. The game will randomly cycle through the available Pokémon.

1. Open your game and collect watts from the den (if not collected already).
2. Use [AutoHost Rolling](https://github.com/PokemonAutomation/Microcontroller/blob/master/Wiki/Programs/PokemonSwSh/AutoHost-Rolling.md) to host!
   > Follow the instruction on the page for correct setup and use.

`Written by doge_stig#9159`
