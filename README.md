# Main Battle Tank (GZDoom)
A main battle tank NPC written in ZScript for GZDoom

Well I don't know what else to say, I had made this months ago but wasn't able to put it up on GitHub due to PC being too old, but now that this isn't an issue, I uploaded it.

Here's a video of an old version of it in action I guess, made with version 1.0 of the tank:

https://www.youtube.com/watch?v=5fwT7eAKW0I

# CHANGELOG

-----|1.2|-----

Additions:

-Added a User_NoCrushing variable, when set to true, the tank will no longer crush NPCs and players in front of it while moving.
-Added a User_NoSmartAim variable, when set to true, the tank will no longer account for its' targets speed when firing.
-Added a User_Stationary variable, when set to true, the tank will no longer move to chase after its' targets.
-Added a User_Fearless variable, when set to true, the tank will no longer move away from a big enough target or a target that is another tank.
-Added the dynamic light and particle spawning that the tank produces when destroyed to its' destroyed props.
-The tanks are now able to fight each other properly, if a friendly tank sees a non-friendly one, it will attack it. The tank shells will phase through tanks that are in the same team, but impact tanks in the opposing side normally.
-If the Dormant, Ambush or Invisible flags are added to the tank through the Edit Thing menu, they will now also be transfered to the turret as well.
-The tank now moves 1.5x faster on Nightmare difficulty or if -fastmonsters is on.

Changes:

-Added some more capitalization in the code for the tank and removed some redundant code.
-Updated the README and also added info on what the two new user variables do.
-Added more editor keys, now the file should load a bit faster, and the decorations will be treated as such by UDB.
-Changed the horizontal scale of the tanks' sprites to 1.2, the tanks' sprites were not made with Dooms' aspect ratio correction in mind, meaning that the tank looked more tall and boxy that its' actual sprites and intended look.
-Changed around the DeathHeight properties of the turret and chassis so they are the same as their normal height. Due to the DeathHeight property setting an actors' height to 1/4th of the original after it dies/is destroyed by default.
-Improved the tanks' retreating, now instead of awkwardly recoiling back when too close to a strong enough target, it'll more properly move away from it instead.
-Renamed ZSCRIPT.DECORATION to Decorations.zsc, and made parsing the code for the tank decorations be done by just using #Include instead of a ZSCRIPT.PREFIX file.

Bugs:

-Fixed the obituaries that the tank produces, now the proper different obituaries are produced depending on whether the player was killed from getting shot or run over by the tank.
-Fixed a bug that caused the tank turret to fixate on specific targets even after they died.
-Not exactly a bug since it didn't cause any issues surprisingly, but the sprite name for the editor sprites of the destroyed tank prop have been renamed from MBTD to MBTR, since MBTD is already used for the destroyed turret.
-Made the tanks' chassis not collide with the turret, allowing the tank to move up and down as it should've.
-Added the NotAutoAimed flag on all the actors related to the tank decorations, so the game won't target them when the player fires.
-Made the frames of the destroyed tank decoration render in full brightness, this was an oversight by me.
-Fixed a bug that caused the tank to be able to fire through walls by getting right up on them and firing, this was extremely annoying to fix and took literally dozens of attempts.
-Fixed a bug that made the tank turret itself count towards the monster count, making it so an enemy tank counts as 2 actors, with the turret never being able to even count as dead. Now it should be properly treated as just one actor.

-----|1.2|-----

-----|1.1|-----
Note: I didn't actually keep track of the changes I made from 1.0 to 1.1, so this is just the changes I've made that I remember, so I've probably made alot of changes that I couldn't remember to list here.

Additions:

-Added destroyed and abandoned/empty variants of the tank, along with user variables to customize each individual decoration. More info on how to use the variables is in the updated README.

Bugs:

-Fixed a bug that caused enemies hit by the tank shells (And survived) to not attack the tank.

Changes:

-Changed the damage of the tank shell itself from 800 to 1000.
-Changed the blast radius of the shell from 256 MU to 500 and the damage from 224 to 256.
-----|1.1|-----
