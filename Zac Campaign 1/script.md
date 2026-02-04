# Mission 1:
### Title: <TBD>
Goal: Plot introduction and familiarization with F22

Starts with tanking - low fuel state and 1 or 2 F22s.   Optionally some F16s.   All planes must refuel.   
Then they're sent to an airfield.   Something seems a bit off but they land.   If there are f16s the base turns hostile and shoots the everliving crap out of them as soon as the F22s are landed.   Marines appear outside the F22 and kill the pilots.



# Mission 2:
### Title: The Heist
Fight or sneak your way to the airfield housing the stolen F-22s.   Either take on enemy fighters or fly stealth with a two ship through a local valley.

With stealth, there's a time limit for all Alpha F16s that are in the game to get there.   Currently set to 5 minutes but that seems long.   A good run is just over 4 minutes.   No SAMs or fighters to fight.   But you still have to deal with ground targets at the airfield.  Perhaps make the ground targets less threatening with stealth.   

Without stealth, you will have to destroy SAM radars as well as enemy 3.5 gen fighters (sparrows/sidewinders) to get in as well as deal with ground targets at F22 base

F16s from Alpha group land and trigger F22 unlock - which also spawns enemy gen5 fighters.   F22s can try to run but any SAM sites that weren't taken out are dangerous (what to do for stealth runs?)   Enemy fighters should be able to catch up to you on your way back especially if you take your time with startup.   

When all F22s are near friendly base then the enemy 5th gens turn around (and also get shot at by friendly SAM sites)

TODO:

1. Disallow the stealth route with more than 2 players
2. Adjust ground spawns based on difficulty a bit further in to the mission - maybe use a path about half way to the F22 base to do the spawn logic based on player count at that point
3. Adjust ground targets at f22 base to be easier with stealth mission "they weren't prepared for us so some systems aren't on"
4. Figure out how to force F22s to take off.   Do they have to taxi?  if so, then the 5th gen figthers need to be moved back.   have to make more barriers to stop them from just blasting off on the taxiway.   "airbase is pretty locked down"
5. Adjust mission to respect "no fail" flag.  Basically just disable the test for losing an F22 and est it to infinite lives.  Is there even a need to limit lives since without the flag the mission ends?
6. Destroy the Alpha F16s when they unlock the F22 (already done?)


# Mission 3:
### Title: Payback
We've located the general viscinity of the GPS spoofers that were used to hijack out F22s.   We need to find the exact locations and destroy enemy defenses.   Then the F22s will strike the 4(?) special hardened targets with their "special penetrator bombs".   A10s will mark targets (probably with laser or whatever mission editor allows) and the "speicial targets" are marked as invulnerable until the mission progresses and alt spawns for the F22s are created with bomb loadout.   Before then F22 may be available for CAP.   F16s are available as well.   F22 will land and swap to another alt spawn that has different weapons available and another life will be provided to allow the respawn to the alt if needed.   

If single player no enemy fighters will spawn or maybe some attack planes will for the A10 to shoot down.   2x A10, 2xF22, 2xF16.  No F22s can be lost.   A10s and F16s can respawn.   


# General Design
Set a GV as the difficulty modifier - set either by picking "MISSION (EASY)" from mission selection or doing something in game to modify the difficulty (like spawning a plane in an alt spawn to set it)
Use player count + modifier to determine difficulty
Then spawn enemies based on modified difficulty GV.

Make a NO-FAIL version of the missions, too - so set a GV on whether failure is allowed and if not and use that in the "failure condition"
