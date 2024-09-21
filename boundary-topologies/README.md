# Boundary topologies

## Neat plate boundaries

When simulating plate tectonics for my world, I got increasingly frustrated by the mess caused by mid-ocean ridges, subduction zones and transform boundaries changing as continents move. 
Looking at [Artifexian's world showcase](https://github.com/akxcv/GPlates-Tips/tree/main/rotation-files), I found a few comments asking how Worldbuilding Pasta managed to create such neat animations of those plate boundary lines, but I couldn't find the answer anywhere.

However, it seems that boundary topologies were used to achieve this.

Here are the screenshots demonstrating this:

> A subduction zone, a transform fault and 2 mid-ocean ridges 990 My ago:
![image](https://github.com/user-attachments/assets/ae9c92c0-0d24-4f02-b2b0-346059805cfc)

> Same features 950 My ago:
![image](https://github.com/user-attachments/assets/2d205cd0-b7b6-4ba3-8922-7325d1a9a099)

> Topological closed-plate boundary 990 My ago:
![image](https://github.com/user-attachments/assets/810baab1-e6da-4777-ba48-542415815541)

> Topological closed-plate boundary 950 My ago:
![image](https://github.com/user-attachments/assets/19c8cd2a-238a-4005-a711-24c13940500e)

## "Teeth" on subduction zones

By the way, to see "teeth" along subduction zones:
1. Subduction zones must have a polarity (`gpml:subductionPolarity`) set to Left or Right.
2. "Teeth" are only displayed in boundary topologies containing a subduction zone.

## Colouring topologies by feature type

In the layer containing your topologies, you can "Set Draw Style" to "FeatureType". By default, GPlates uses [its own feature type colour palette](https://github.com/GPlates/GPlates/blob/gplates/src/gui/FeatureTypeColourPalette.cc), however, if you're like me and you're used to the colour palette from [Worldbuilding Pasta's articles](https://worldbuildingpasta.blogspot.com/2020/01/an-apple-pie-from-scratch-part-va.html), you can make your own palette (see the example file in this repo). In "Set Draw Style" -> "FeatureType", click "Add", then "Open..." in the "Palette" row, and attach your own `.cpt` file.
