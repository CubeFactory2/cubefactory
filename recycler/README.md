# Recycling unit
## Overview

 The recycling unit of the cubefactory 2 is able to produce filament for the 3d printer. In a two-step process plastic waste is shred into little pieces and then transformed into filament.

+ __Input:__ waste from 3d printing or other plasic e.g. from plastic bags or plastic bottles (just a single type of material)

+ __Output:__ filament that can be (spooled an then) used for FDM 3d printing 

+ Two-step __process__ realized by two independent __modules__: 
	1. Shredding the material into small pieces ([shredder](#Shredder)) 
	2. Extruding the filament ([extruder](#Extruder))

+ The [powertrain](#Power) module can be attached to either the shredder or the extruder with the purpose of saving weight and costs

+ Special requirements for the recycler to be used in the cubefactory 2:
	+ To be compact (small package)
	+ To be lightweight
	+ Low power consuption 

+ Hierarchy and foto of the realized construction (3d view [here](CAD/CAD(stl)/00_00_00-wecycler.STL)):

 ![Overview Structure of Repo and Construction](images/WeCycler_structure.png)
![Bild Zeichnung WeCycler](images/wecycler_foto.jpg)

## Shredder <a name="Shredder"></a>
### Goals and concept
The Shredder aims to mechanically shred the input material into small, similar sized pieces.

+ __Input:__ 
	+ Different plastics (as long as they are sorted, clean and dry)
	+ Possible sources could be misprints or PET bottles
+ __Output:__
	+ Smaller pieces (pellets)
	+ Pieces should hopefully be equally sized (to later get a more consistent filament)
	+ Maximum size can be limited via usage of filters
	
+ The selected __principle__ is a cutting mill with a stator and a rotor both equipped with static/ rotating blades 
+ The shredder should be __adaptable__ to process different materials and deliver variable pellet sizes
![Schneidmühle Prinzipskizze](images/Schneidmuehle_prinzip_quelle.jpg)

### Realization
![shredder](images/shredder2.png)
+ The rotor is realized by a used (and damaged) milling cutter  (recycling!) 
+ The other parts are special components that have been manufactured for the WeCycler
+ To adapt to different materials, the speed (rpm) of the rotor is adjustable. Furthermore static blades can be moved to to change the distance between static and dynamic blades.
+ The output pellet size is determined by selection of a changeable filter (perforated plate)
+ More detailed information about the realized shredder [here](Shredder_Info.md)
 
## Extruder <a name="Extruder"></a>
### Goals and concept
The extruder produces filament from pellets using pressure and heat.

+ __Input:__ pellets or shredded material (equally small sized and just one type of material)
+ __Output:__ filament
+  The extruder __process:__ [(explanation video)](https://www.youtube.com/watch?v=WaB-dsB1Kfk)

	1. Feeding the material into a hopper
	2. The pellets are moved through a tube by a spinning screw
	3. The plasic melts due to the use heating elements along the tube an the pressure resulting from decreasing distance between screw and tube
	4. Finally the meltet material is pressed trough a nozzle, forming a string of filament
	 
+ The extruder should be __adaptable__ to process different materials and pellet sizes. Also the diameter of the filament should be variable.

(__TODO__ Bildquelle))![Extruder Prinzipskizze](images/Extruderschema2.jpg)

### Realization 
(__TODO__ Bildquelle, Beschriftung der Einzelteile?))![Extrudergruppe](images/Extruderbaugruppe.jpg)

+ More detailed information on the single parts of the realized extruder unit [here](Extruder_Info.md)
 
## Powertrain <a name="Power"></a>
+ For more information on the powertrain unit see [here](Powertrain_Info.md).
+ The powertrain can be attached in 2 different positions: either it drives the the shredder (pink) or the extruder (green). This is due to the need of saving money, space and weight.

![positions](images/powertrain_positions.jpg)
### This Repository
+  Exploded views [here](CAD/exploded_views)
+  BOM [here](BOM)
+  CAD files [here](CAD)

### More Information
+ https://www.3dhubs.com/talk/thread/which-shredding-and-extruding-machines-are-available-part-3
+ https://www.3dhubs.com/talk/thread/how-does-local-recycling-work-part-2
