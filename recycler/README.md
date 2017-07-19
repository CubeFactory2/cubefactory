###TODO (texting)
+ [x] Overview (hier kurze Einführung zum [Recycler] (#Recycling-Unit))
+ [ ] Shredder
	+ [ ] Shredder concept
	+ [ ] Shredder realisation
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


## Shredder <a name="Shredder"></a>
### Ziel und Prinzip
* mechanisches Zerkleinern von (sortenrein?) Material, Fehldrucke oder PET Flaschen
* es entstehen Pellets
* verschiedene Materialien möglich
* verschiedene Zielgrößen der Pellets möglich
* Konzept der Schneidmühle (cutting mill: (__TODO__ Bildquelle))![Schneidmühle Prinzipskizze](images/Schneidmuehle_prinzip_quelle.jpg)  
### Der verbaute Shredder
- solche infos:
2500 RPM | Torque: 26.5 Nm | Chamber Size: 7.75" | Sample Volume: 50 - 1000g

- alter wälzfräser
- 
## Extruder <a name="Extruder"></a>
### Das Prinzip Extruder

* Filament herstellen aus Pellets
* Extruder heißt ... Druck, Temperatur
* Pellets könnten auch einfach gekauft sein (billiger als gekauftes Filament)
* 3-Zonen-Extruderschnecke mit kernprogressivem Verlauf, Thermalbarriere
* 
(__TODO__ Bildquelle))![Extruder Prinzipskizze](images/Extruderschema.jpg)

### Der verbaute Extruder 
Sieht so aus: (__TODO__ Bildquelle, Beschriftung der Einzelteile))![Extrudergruppe](images/Extruderbaugruppe.jpg)

### Powertrain <a name="Power"></a>

### Dieses Verzeichnis
+  explodes views [here](images/exploded_view)
+  BOM [here](BOM)
+  [CAD files](CAD)

###Links
https://www.3dhubs.com/talk/thread/which-shredding-and-extruding-machines-are-available-part-3
https://www.3dhubs.com/talk/thread/how-does-local-recycling-work-part-2
