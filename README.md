# On the Importance of 3D Printed Game Organizers
Merry Christmas, Dad! You'll notice that Mom got Cascadia and the Landmarks expansion. Great! The only issue (trust me, this is definitely a _real_ issue and not something I've contrived) is that the game doesn't come with a great way to store its components. Plastic bags can get annoying, and having to store cards in bags just feels downright wrong to me. Not to worry! Making small components that vastly improve your everyday quality of life is exactly what 3D Printers were made for, and it's an area where they excel. What I've made here is a small document that should walk you through the basic steps of setting up and printing your very own Cascadia Organizer. 

Hooray!

This file, and all others mentioned are available at https://github.com/sredna43/Christmas-3D-Printing-Guide.
## Software
You'll need the following apps:
1. A CAD program (I use [Autodesk Fusion for Personal Use](https://www.autodesk.com/products/fusion-360/personal))).
2. A slicer (I use [Orca Slicer](https://github.com/SoftFever/OrcaSlicer/releases/latest), a fork of Bambu Studio).

You already know what a CAD program is, and I assume you know how to use one (probably much better than I do). I will tell you this, however, I design parts that need to fit together to a 0.15mm tolerance minimum and this seems to work well for my applications.

A slicer takes an exported 3D object (I always save my meshes as `.stl` files) and converts it into G-Code which the 3D printer understands. I doubt you've used a slicer much, so that's mostly what I'm going to focus on for this guide.

## 3D Models
Now that you've downloaded your CAD program and slicer (you did do this, right? You're not skipping steps?) you can either create your own organizers from scratch or use the [ones I designed for you](https://github.com/sredna43/Christmas-3D-Printing-Guide).

If you choose to create your own, I've gone ahead and measured out the sizes for the cards and roughly estimated how much size the other components need:
### Measurements
Box Interior: `230mm x 230mm x 67mm`
Instructions: `230mm x 230mm x 2mm`
Base Game Score Pad: `160mm x 65mm x 7mm`
Landmarks Score Pad: `175mm x 88mm x 7mm`
Animal Scoring Cards: `120.60mm x 70.50mm x 13.25mm`
Landmark Scoring Cards: `67.20mm x 44.10mm x 21.50mm`
Nature Tokens (roughly): `70mm x 50mm x 25mm`
Landmarks (Roughly): `120mm x 70mm x 50mm`
Staring Tiles: `3, 25mm sided hexagons arranged in a triangle`
Habitat Tiles: Frankly, whatever room is leftover in the box.

## Slicing
We have our models, either designed or downloaded, let's turn these meshes into a language the printer can understand; a series of nozzle head movements and extruder... extrusions? I'll try to give an overview of the steps below.

1. Export the meshes as `.stl` files. In Fusion, I do this by right clicking the body I want to export under the component tree on the left and selecting "save as mesh". Make sure you save it as a `.stl binary`. 
2. Open up your slicer program
3. Click "new project"
4. Press `ctrl + I` or click on the cube with a plus sign in the top toolbar to add a new object
5. Select the object you want to print, and import it onto the build plate (for demonstration's sake, I'll use the `Starter Tiles.stl` file).
6. Select the "0.20mm Standard @BBL X1C" profile from the dropdown in the left menu above the "Quality, Strength, Speed, etc" tabs.
7. Orient the object for printing, following these general principles:
	1. Minimize overhangs (our printer is really good, but it can't print in thin air yet).
	2. Minimize the need for support (it's fine to have some, but in general I try to design and place my objects in ways so that they don't need much support).
	3. Best practices say to only print one object at a time, I never follow this one
8. Press "Auto Orient objects on plate" next to the build plate (an A in a box) to do all of step 6 automatically.
9. Enable support
	1. In the left menu, navigate to the "support" tab
	2. Check "enable support"
	3. Change type to Tree(auto)
	4. Leave style as default
10. Press "slice plate"
11. Make sure there are no errors, and that the object looks normal
12. Press "print plate"
13. Wait for the part to be done printing!

## Printer Basics
Our printer is as close to "Plug and Play" as a 3D printer can possibly be. Realistically, all you need to do is load it up, clear off the build plate of any debris from old prints, and hit send from the slicer. However, if you ever need to load in new filaments or want to play around with other features let me know and we can figure it out together!

Happy Printing!

