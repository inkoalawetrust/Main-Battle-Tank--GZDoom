Credits for the sound sources are included inside the .pk3 itself.
Sprites: Made by Gorman Freebmane, edited by me.
Code: Written by me, A_IsPlayerClose function made by Agent_Ash.

The tank has 5000 HP (1000 more HP than the Cyberdemon) each tank shell does roughly 1200 damage and exactly 1000 damage from the projectile itself.

Editor keys are included, which means that the tank can be found under a "Vehicles" folder in the Edit Thing window. You can also spawn the tank directly in-game by typing "summon mainbattletank" in the console, or "summonfriend mainbattletank" to spawn a friendly tank. Setting the tank to friendly in the editor should work as well.

================|USER VARIABLES|================

If you don't know how to use and/or change the user variables of an actor, then click on this Imgur album to see how: https://imgur.com/a/IF9Ezo2

USER VARIABLES FOR THE TANK ITSELF:

User_NoCrushing: When set to true, the crushing damage the tank performs to NPCs/monsters and players when moving will be turned off.

User_NoSmartAim: When set to true, the tank will no longer take its' targets velocity into account when aiming and firing at them.

User_Stationary: When set to true, the tank will not move to chase after a target and simply stand still and shoot, similar to the tanks in Half-Life 1.

User_Fearless: When set to true, the tank will not move away from its' target if it is above a certain size or is another tank.

TANK DECORATION USER VARIABLES:

Note: Both the destroyed and empty/abandonded tank have the same user variables.

User_TurretAngle: An interger that changes the turrets' angle relative to the angle of the chassis, can use negative values to rotate the turret left or right.

User_RandomTurretAngle: When set to true it will set the turret at a random angle relative to the chassis, and overwrite User_TurretAngle.