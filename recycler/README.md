### TODO (texting)
+ [x] Overview (hier kurze Einführung zum [Recycler] (#Recycling-Unit))
+ [x] Shredder
	+ [x] Shredder concept
	+ [x] Shredder realisation
+ [ ] Extruder
	+ [ ] Extruder concept
	+ [ ] Extruder realisation
+ [ ] powertrain (>Ali)

 
-------------------------------------------


# Recycling Unit
## Overview

 The recycling unit of the _cubefactory 2_ is able to produce filament for the 3d printer. In a two-step process plastic waste is shred into little pieces and then transformed into filament.

+ __input:__ waste from 3d printing or other plasic e.g. from plastic bags or plastic bottles (just a single type of material)

+ __output:__ filament that can be (spooled an then) used for FDM 3d printing 

+ two-step __process__ realized by two independent __modules__: 
	1. shredding the material into small pieces ([shredder](#Shredder)) 
	2. extruding the filament ([extruder](#Extruder))

+ the [powertrain](#Power) module can be attached to either the shredder or the extruder with the purpose of saving weight and costs

+ Special requirements for the recycler to be used in the _Cubefactory 2_:
	+ to be compact (small package)
	+ to be lightweight
	+ low power consuption 

+ hierarchy and drawing of the realized construction (3d view [here](CAD\WeCycler\Extrudergruppe\Extrudergruppe_STL\Baugruppe)):

+ ![Overview Structure of Repo and Construction](images/WeCycler_structure.png)
![Bild Zeichnung WeCycler](images/WeCycler_drawing.jpg)
+ __TODO__ bessere Abblidung (aus CAD? )

## Shredder <a name="Shredder"></a>
### goals and concept
The Shredder aims to mechanically shred the input material into small, similar sized pieces.

+ __input:__ 
	+ different plastics (as long as they are sorted, clean and dry)
	+ possible sources could be misprints or PET bottles
+ __output:__
	+ smaller pieces (pellets)
	+ pieces should hopefully be equally sized (to later get a more consistent filament)
	+ maximum size can be limited via usage of filters
	
+ the selected __principle__ is a cutting mill with a stator and a rotor both equipped with satic/rotating blades 
+ the shredder should be __adaptable__ to process different materials and deliver variable pellet sizes
(__TODO__ Bildquelle, übersetzen))![Schneidmühle Prinzipskizze](images/Schneidmuehle_prinzip_quelle.jpg)


### realization
+ picture shredder __TODO__ (erstellen aus STEP/SLDPRT)
+ the rotor is realized by a used (and damaged) hob cutter  (recycling!) 
+ picture hob cutter __TODO__ (aus masterarbeit)
+ To adapt to different materials, the speed (rpm) of the rotor is adjustable. Furthermore static blades can be moved to to change the distance between static and dynamic blades.
+ The output pellet size is determined by selection of a changeable filter (perforated plate)
+ __TODO__ solche infos finden :
 2500 RPM | Torque: 26.5 Nm | Chamber Size: 7.75" | Sample Volume: 50 - 1000g
 
## Extruder <a name="Extruder"></a>
### goals and concept

* Filament herstellen aus Pellets
* Extruder heißt ... Druck, Temperatur
* Pellets könnten auch einfach gekauft sein (billiger als gekauftes Filament)
* 3-Zonen-Extruderschnecke mit kernprogressivem Verlauf, Thermalbarriere
* 
(__TODO__ Bildquelle))![Extruder Prinzipskizze](images/Extruderschema.jpg)

### realization 
Sieht so aus: (__TODO__ Bildquelle, Beschriftung der Einzelteile))![Extrudergruppe](images/Extruderbaugruppe.jpg)

### Powertrain <a name="Power"></a>

### Dieses Verzeichnis
+  explodes views [here](images/exploded_view)
+  BOM [here](BOM)
+  [CAD files](CAD)

### Links
https://www.3dhubs.com/talk/thread/which-shredding-and-extruding-machines-are-available-part-3

https://www.3dhubs.com/talk/thread/how-does-local-recycling-work-part-2
