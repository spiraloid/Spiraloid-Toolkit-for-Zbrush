# Spiraloid-Toolkit-for-Zbrush
Custom UI, hotkeys and colors for Zbrush 2019.

this makes me a lot faster and I never hit the zadd, zsub, m, rgb etc buttons because of it.  I like to bind right click for my mouse and stylus to "u".

https://spiraloid.github.io/Spiraloid-Toolkit-for-Zbrush/

WARNING:

this is my personal workflow setup, no support, liability or warranty should be assumed.  I'm just sharing my setup.  if it breaks yours.  bummer.  be warned.

Usage:

this creates a spiraloid menu that is bound the "u" hotkey.  
I suggest mapping this key to the back button on your mouse and a wacom pen side button. 

once installed, you should never have to press zadd mrgb etc.  if you need to, it's still availiable on right click or spacebar.

press setup in top right each time you open a project to reset camera behavior, initialize settings and activates a timelapse recording.

press nuke in top right to erase the polypaint and flood the current subtool with 50% gray and material.


Installation:
-extract the "Spiraloid" folder in this location.  C:\Program Files\Pixologic\ZBrush 4R8\ZStartup\Macros\

-restart zbrush.

-Press menu macros > "Reload all Macros".

-Press menu macros > Spiraloid > "_______________Install_______________"  button at the bottom.

-Press preferences > Config > "Store Config" (assuming you want to keep using it after restarting ZB)

-Press preferences > Hotkeys > "Store Hotkeys" (assuming you want to keep using it after restarting ZB)



Caveats:

everybutton is a macro with varying levels of zScripting in them and has been tuned from years of use.

changes from the default hotkeys:

ctrl d : deselects mask

ctrl h : hides mask

ctrl i : inverts mask

shift c : frames tool

ctrl e : merges subtool down.

ctrl f : flood color

shift F :  toggles wireframe and solo at the same time. super useful for live boolean object editing.

ctrl g : polygroup visible

f : toggle wireframe

1 : flat shade

2 : preview shade 

3 : skin shade 

4 : clay shade 

5 : pewter shade 

6 : toon shade 

7 : render w rimlights and AO

f4 : automesh current subtool.  this remeshes to 1000K polygons, subdives 5 times then projects the shape and polytpaint from the original mesh before deleting it.  (hit yes to project and delete)  Sadly this has no UV's since I can't zscript or macro any plugins (like decimation master or fbx exporter).

alt-s : smooths unmasked parts of the mesh.

shift f : toggles wireframe and solo together, usefull a live boolean invert with zmodeller.

insert : add new layer, prompt for name, set to 1 and record.  *note every layername must be unique. if your arrow keys stopped working it's because two layers have the same name.  zscript limitation.

left arrow: previous layer and enter record mode.  good for flipbook sculpting animations or face shapes.

right arrow: previous layer

up arrow : toggle base edit vs current layer sculpting.  beware changes to the base effect all layers. 

ctrl c : copy shape (stores morph target)

ctrl v : paste shape (switches current shape for stored morph target, then activates the paint morphtarget brush to paint back to the stored shape)

