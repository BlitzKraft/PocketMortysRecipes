Easily accessible list of pocket mortys recipes.

A total of 40 items. Primary: 10; Craftable: 30.

~~All words are in CamelCase. Yes, the first character of the first word is capitalized too.~~  
Although true, it is not relevant anymore due to fuzzy match.

###Depends:
networkx - This is meant as an exercise to use and get familiar with this library.  
This could be (probably easily) be done even without using that.

fuzzywuzzy - For fuzzyfind. If you choose not to use it, read the `recipe` and modify the file as specified.

###Usage:
`./recipe <item>`

`<item>` is what you are trying to craft. Case insensitive. ~~Exact string match~~. Fuzzy match. Following are all craftable items.

 - MortyManipulatorChip
 - Serum
 - GreatSerum
 - SensationalSerum
 - PureSerum
 - PlutonicRock
 - PurePlutonicRock
 - Halzinger
 - PureHalzinger
 - LevelUpMegaSeed
 - Battery
 - SuperchargedBattery
 - MicroverseBattery
 - PurifiedFleeb
 - MutantBacteriaCell
 - DarkEnergyBall
 - DarkMatterBall
 - Motherboard
 - DogCollar
 - LovePotion
 - Robot
 - ButterRobot
 - GwendolynDoll
 - TimeCrystal
 - TimeStabilisingCollar
 - InterdimensionalCblBox
 - NeutrinoBomb
 - InterdimensionalGoggles
 - IQEnhancingHelmet
 - RoyVRHeadset

###Recipes:
New recipes can be added by simply appending them to `pure.list`. Then run `./generate test` (optional) and `./generate write` to save the results. The first item is the goal and the rest are its constituents.  
Example line from the file would be:  
`GwendolynDoll			Robot				LovePotion`  
The number of tabs is irrelevant. However, there shouldn't be spaces. The script exclusively tests for tabs and **not** spaces. 

This however does not update the `recipes.list`. This has to be done manually. This file is for human reading and not just parsing. Ergo, it should be hand tuned for readability.

This is done for future proofing. Potentially more recipes could be revealed in later updates of the game. Then, I will be ready.

If an item is not craftable, it outputs nothing. By default battery and supercharged battery are included in basic items, by appending to the list, to reduce output clutter. This behavior can be disabled by commenting out the specific lines. 
