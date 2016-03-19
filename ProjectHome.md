_[You may also want to take a look at my HUD for TF2](http://code.google.com/p/broeselhud/)_

# General Info #

This is a simple Script that allows you to switch between crosshair- and viewmodel-settings for each slot and class individually. It also doesn’t show the behaviour of other crosshair switcher scripts to screw up lastinv (Q).

Whereas other crosshair switcher scripts just switch between slot1 and slot 2 when you press Q or whatever key you have bound lastinv to, this script executes the lastinv command just like 'normal TF2'.

Also, this script allows you to change the slots in the quickswitch menu with the number keys (doesn't work in other scripts) and switch weapons while looking at the scoreboard.

To customize your settings, the script offers a clearly arranged settings file, that allows you to use preset aliases for colors, shapes and sizes.

**You can download the Script here: http://code.google.com/p/broesels-crosshair-switcher/downloads/list**

**a changelog can be found here: http://code.google.com/p/broesels-crosshair-switcher/wiki/Updates

---

# Installation #**

To install the Crosshair Switcher, extract the cfg folder to:

`Program Files\Steam\steamapps\<user name>\team fortress 2\tf\`

### REMEMBER TO BACKUP YOUR CLASS CFG'S BEFORE INSTALLING THE CROSSHAIR SWITCHER, IF YOU HAVE ANY CLASS-SPECIFIC SCRIPTS IN THERE! ###

---

# customize your crosshairs #

open cfg/crosshairswitcher/settings.cfg and edit the aliases
there which are following this syntax:

`<class>_<slot> "size; color; type; viewmodel FOV or viewmodel off"`

to your liking. At the top, you also find 3 presets you can change.

### Disabling the script for certain classes: ###

To disable crosshair-switching for a class, simply change this in the class cfg file:

`exec crosshairswitcher/switcher -> exec crosshairswitcher/disable`

When disabling the switcher, the crosshair that you specified for the primary slot
of this class will be used.

Per default, the switcher is disabled for Heavy, Engie and Spy to prevent minor,
unavoidable glitches.

---

# customize your binds #

open cfg/crosshairswitcher/binds.cfg and change the binds for the functions
listed there to your liking.

I've already made a section under the default binds which sets the script to
select slot1 on mousewheel UP, slot2 on mousewheel DOWN and slot3 with the
upper thumbbutton.

To use this alternate bind-config, simply uncomment the whole section and leave
the upper one - it will then overwrite the default settings.

If you want to have the lastweapon command just switch between your primary
and secondary weapon, uncomment the last section and change q to something else
if you prefer a different key.

---

# Integration of other scripts #

If you have any other scripts, insert them into the class cfg files
from your backup. Note that to work correctly, they will now require
weapon1 instead of slot1 and so on - otherwise your scripts will just
change the slot and not the crosshair.

To do this, simply do "search and replace" in your text editor and
let it replace all "slot"'s with "weapon"'s.

You don't have to do this for classes where you disabled the crosshair switcher.