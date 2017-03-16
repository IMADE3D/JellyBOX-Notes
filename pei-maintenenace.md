# Heated Bed Quick Start

Congratulations. You have just acquired a powerful weapon to help you with **your war on warp**: the JellyBOX heated bed upgrade. This short document will help you get the most out of it.

## Guidelines
- Your heated bed is limited to **80C**, and for most materials under most conditions, you won't need to go above **55C**. High enough a temperature to print a wide range of materials with no warp, but low enough to prevent burns, and keep the JellyBOX friendly.
- You can use heated bed with any material and any print surface (/treatment), but some combinations are better than others.
- **PETG**.
  - PETG on a heated PEI sheet is a wonderful combination. You will like it. You may find you even have to increase your nozzle distance if it sticks too well.
  - PETG on blue tape works quite well, but warps more than PLA.
- **PLA**.
  - For PLA on PEI sheet, 45C is a good ballpark. Most users do not have good luck with PLA on cold PEI. Some even claim one has to use PVA base glue stick. (We have been printing without glue stick successfully.)
  - _PLA does not usually require heated bed_ when used with blue tape. Don't get me wrong, heated bed still reduces warp, but PLA often warps so little (even when using just plain blue tape), that the additional time spent on heating the bed is not worth it for many users. However, in colder environments, you can use the heated bed to get to pleasant 25C.
- (Nylon.)
  - Experimental. Usable with PVA based glue stick, but we need more experiments to determine the best settings.
- (ABS.)
  - We do not officially support ABS. When ABS melts, it produces fumes that seem to harmful to humans. The research is still not conclusive, but we err on the side of caution. The good news is there are many materials today that are superior to ABS mechanically, and are easier to print. Use PETG instead! If you really want to, you will be able to print ABS on the JellyBOX, but... you'll have to figure that out.

# PEI Sheet Usage and Maintenance
- PEI (Polyetherimide) is the king and queen of heated bed surfaces. Almost maintenance-free, produces smooth, glass-like first layers, it works with a wide range of materials (PLA, PETG...) and can lasts for hundreds of prints.
- PEI sheet needs to be heated up while printing, but it often needs to cool down a bit before you take the prints off.

## Degreasing and Maintenance
- You have to keep your PEI sheet clean. Human fingers and skin are greasy, so try not to touch the surface.
- Wipe the surface with **isopropyl alcohol** before print to clean it off any grease and dirt.
- You don't have to wipe off the surface with alcohol before every print as long as you don't touch it. Additionally, wipe the tools you use to separate the prints isopropyl alcohol as well.
- The adhesion may be too strong for some PETG and TPU blends; you may need to set your nozzle higher for the first layer than you're used to.
- Alternatively, you can use window cleaners (alcohol based) or dish soap and warm water.
- You can clean the surface while it's hot; just don't touch it with your greasy fingers or dirty tools.
- You can also occasionally use high grit (1500+) sandpaper to gently remove scratches and restore the surface. After you do this several times, you may need to replace your PEI sheet.

## Removing Finished Prints

### School of though 01: cool it off
- Practiced by most
- Prints are easiest to remove when the part AND the bed cool down.
- > If you are impatient, For persnickety parts, let the plate completely cool and pop them off or, if really persnickety, put the plate and part in the freezer. That will ALWAYS work. I'm too impatient for that so I use a can of electronics freeze spray. You don't have to chill the entire part, simply aim at an edge attached to the PEI and squirt. [~ mhackney](http://sublimelayers.blogspot.com/)
- > [If it's really stuck.] No problem. While the print is cooling, apply some alcohol - any type -- around the edges of the print. Capillary action pulls the alcohol in and POP! the print just floats free without any need to pry or apply any force at all. It is really that easy. It may take 30 seconds or several minutes. If the print cools, heat the bed back up to about 60C and turn it off and then apply the alcohol. You will hear pops and cracks as it comes loose. The you reach down and find it is actually floating on top of the plate completely unstuck. Yeah! [~JohnSays](https://www.thingiverse.com/groups/da-vinci/topic:5059)

### School of thought 02: 50C-60C
- As reported by Lulzbot support
- Prints are easiest to remove when they bed is between **50C and 60C**.
- You can modify your end gcode to keep the bed at this temperature range for a while after the print finishes before completely turning off the bed:
```
M140 S58            ; bed heater lower temp (if you have it)
G4 S300             ; wait 5 minutes
M140 S0             ; bed heater off (if you have it)
```
- Use thin painter's knife to separate the prints.
-  Do **not pry**, but rather **separate** the finished print.


## Cold Environment
- Try increasing bed temperature. That usually helps. Even 80C for PETG if you have to.
- In cold environments, warp is worse as the temperature gradient is bigger. (Cold environment is anything below 21C, but we have had printers in rooms as cold as 10C.)
- Try to enclose the printer to decrease cold air flow. Old wardrobes work great!

## Replacing PEI Sheet
- PEI sheet can last hundreds of almost-maintenance-free prints, but it will eventually wear down. (Especially if you drive your nozzle too low) 😼
- With some effort and elbow grease, you can replace the sheet yourself. Get in touch to get a new PEI sheet with the proper industrial strength glue to keep it on the bed.
