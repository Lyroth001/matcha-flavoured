# matcha-flavoured backport
## What is this??
This is a backport of version 1.12.2 of the minecraft 26.2 datapack Matcha Flavoured by Klei_Wright, the original of which can be found here: https://github.com/kleiwright/matcha-flavoured. If you have somehow managed to find this with no idea what Matcha Flavoured is, go watch Klei's video on it here: https://www.youtube.com/watch?v=zyRH8W58fRI.

## What is the point of this
Great question! Matcha Flavoured is an excellent modpack which strongly aligns with many of my design feelings with regard to Minecraft and the various flaws present in the vanilla game, however versions beyond the original alphas are only compatible with minecraft 26.2. While this is fine if you want to play the pack by itself, the many content-focused mods are not updated to 26.2. (I mean. A lot of the mods I'd like to use are not on 26.1.2 either but I digress, at least there are some :p )

## That sounds great!! How do I install this?
Clone or download the repo (big green button that says code, download as zip)
1. Extract Matcha_Flavoured_Backport
2. Compress it to a zip
3. Put that in your worlds datapacks folder 

## Changes from the original
This is an in-progress work as I play through the datapack with my custom modpack, and as such there is **absolutely no guarantee of stability or bug freeness**. In that spirit, there have been a handfull of changes made due to the backport that cause mechanical changes, as I have been unable to figure out a fix without this. They are listed here, alongside any relevant instructions for mitigating the change.
#### 1. Mobs will not stop spawning after killing the dragon
I have ran into the issue where gamerule_safe_surface procs too early after killing any mob, and my attempts to fix this have so far failed. As such, the function that checks this gamerule has been disabled. If you wish to reenable this, uncomment the 2nd line of `data/main/function/mechanic/spawn_mechanic/ticking.mcfunction`

## Will this be updated for newer versions of the datapack?
Probably, if I am still interested in playing it and it isn't a massive PITA to do (She says, nervously eyeing the namespace changes occuring in the upstream repo).

## Will you also do this for x version of Minecraft?
No. The backport here has been relativly easy so far, since there have only been minor changes between the two versions. Older versions introduce significantly more breaking changes and I am not about to manually recode all the items, or create a tool for that. 