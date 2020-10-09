This is most of Rob's scripts for TT++, plus a tmuxinator file that often screws up the layout slightly.
You may need to practice your commands for swapping windows around in TMUX just in case.

I was using an (incomplete!) external mapper rather than the TT++ mapper, so I don't actually have
any mapper support in here.

It should load 5 windows if you use tmuxinator. You'll likely have to tweak font size to deal with minimap.
Main
Minimap
Status Window
Chat log
CP/GQ mob list

The last 3 have files that are dumped to disk by TT++, and the shell script will watch those files for changes.


Setup:
> Edit up setup.tin (it needs the path to the directory with all the .tin files)
> Edit variables.tin a little 
   > Change the names of potions you're carrying so it can track them
   > There should be an alias to update the name of your midround attack, there is a doodad to auto-cast/attack during combat.
     (it also has a variable to adjust the seconds of lag from your attack to tune it, sometimes 3 sec, sometimes 4)


Rob's preferred commands, some aliases might need tweaking:
qa <mobname> (attack a mob with your preferred attack)
as (use your midround attackskill)
attackskill <skill or 'cast spellname'> - set what you want to do in midround
fb (cast fire breath)
opa (open doors in every direction)
ah <keyword> (auto-hunt for a mob)  - Probably need to add a way to cancel it, usually I end up 'ah sldjkfhasc' to stop it if it gets stuck in a loop.
chmob <keyword> (auto-hunt, but 'charge' one step in the direction), I use this in 9hells a lot.
ahpet (auto-hunt for your pet, gotta have your pet name saved)
ht <keyword> (hunt trick. Good for CPs yet, but useless for GQ)




