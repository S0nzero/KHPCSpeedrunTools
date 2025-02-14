How to use:
- Get LuaBackend https://github.com/Sirius902/LuaBackend
- Follow its instructions on how to setup scripts and they will run automatically with the game

SaveAnywhere:
- In-game, press L1+L2+R2+Select (or equivalent on your input device)
- You can use this to save anywhere. Saving during cutscenes or combat may have unexpected consequences.
- You can also instantly die with R1+R2+L2+Select
- You can also instantly load continue state with R1+R2+L1+L2+D-pad left
- You can also instantly load autosave with R1+R2+L1+L2+D-pad right
 - Most recent continue state is written to a local file that carries between restarting the game
 - Can be loaded straight from the title screen
 - The save can be found in the Lua .exe/.dll folder
 - Might have weird bugs, might save you from losing a lot of progress
- You can also soft reset with R1+R2+L1+L2+Start

InstantGummi:
- Instantly arrive at any selected world
- Warp points are disabled
- Warp drive is disabled (it'd be slower)
- Attempting to travel to Halloween Town or Atlantica will take you to Monstro if it has not yet been visited
- To go to Hollow Bastion 2, select the warp point that takes you there
- There is a possibility that going to Deep Jungle or Neverland for the first time will not initiate the opening cutscenes. In this case, report the issue. You can progress the game by going to treehouse/cabin

Unskippable:
- Allows skipping unskippable cutscenes (Wonderland, HB2)
- Can not skip text boxes or "mini cutscenes" such as drinking enlarge/shrink potions in Wonderland

EarlySkip:
- Allows skipping cutscenes earlier
- May cause glitches

FasterDialog:
- Makes text boxes appear and disappear almost instantly
- Text speed unaffected unless you change textSpeedup to true (line 2)
 - This feature is a little wacky so it's disabled by default

FasterAnims:
- Speeds "mini cutscenes" as well as room transitions
- Also speeds up summon animations. If you don't want that, replace "summonSpeedup = true" with "summonSpeedup = false"
- Default speed multiplier is 2.0, but you can change it to anything you like

Autoattack:
- Holding down attack allows Sora to perform physical attack combos automatically
- This will guarantee very quick combos
- Made for accessibility reasons

RandoSomeLogic:
- Randomizes items, level ups, rewards, magic, trinities and chests
- If seed.txt exists, it will try to use it. Otherwise, the file will be created with a random seed.
- randofiles folder should be placed in the same folder as the .dll when using Luabackend Hook by Sirius
- Combine with SaveAnywhere and InstantGummi to get to world map right away. Everything will be open.

EnemyRando:
- Randomizes most bosses and some enemies within restraints of (hopefully) not crashing
- If seed.txt exists, it will try to use it. Otherwise, the file will be created with a random seed.
- randofiles folder should be placed in the same folder as the .dll when using Luabackend Hook by Sirius
- Scales bosses to match the location
- Probably has some issues. Send enemyrandolog.txt from randofiles folder and description of issue.
- Hold start and only start during all black screens to skip randomization of that room.

Chaos:
- Randomizes many things in wild, chaotic ways, including attack animations
- Use for silly times

ConsistentFinishers:
- Makes Zantetsuken, Gravity Break and Stun Impact trigger 100% of the time
- Priority: Stun Impact -> Gravity Break -> Zantetsuken

Unlock0Volume:
- Setting BGM volume to 1 mutes it

FastCamera:
- Speeds up the camera and its acceleration
- Makes camera centering instant
- You can adjust the numbers in the script to your liking

4By3:
- Sets the aspect ratio of the game to 4:3
- You can set the resolution via display settings or by resizing the window directly. That height will be applied and width cut to match 4:3
- Visit display settings to get rid of black bars
- Menus appear slightly cut-off since they were made for 16:9

1HP:
- Forces Sora's max HP to 1 at all times
- Removes beeping noise.

Achievements:
- Displays in Lua console when you get achievements and overall progress, independent of EGS achievement progress
- Saves achievements locally in achievements.txt, in game install folder or Lua .exe folder depending on Lua program
- Delete achievements.txt to reset achievements