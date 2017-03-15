# Pei Maintenance
(Heated Bed Use Guide)

## PLA
PLA does not usually require heating on PEI, but 45C can be good to further combat warp.

## PETG
- PEI is a great surface for PETG.
- You need to heat up the bed to about 55C (environment dependent) to get good results.

## Degreasing and Maintenance
- You have to keep your PEI sheet clean. Human fingers and skin are greasy, so try not to touch the surface.
- Wipe the surface with **isopropyl alcohol** before print to clean it off any grease and dirt.
- You don't have to wipe off the surface with alcohol before every print as long as you don't touch it. Additionally, wipe the tools you use to separate the prints isopropyl alcohol as well.
- The adhesion may be too strong for some PETG and TPU blends; you may need to set your nozzle higher for the first layer than you're used to.
- Alternatively, you can use window cleaners (alcohol based) or dish soap and warm water.
- You can clean the surface while it's hot; just don't touch it with your greasy fingers or dirty tools.
- You can also occasionally use high grit (1500+) sandpaper to gently remove scratches and restore the surface. After you do this several times, you may need to replace your PEI sheet.


## Removing Finished Prints
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
