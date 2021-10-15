# IoC_Circuitscape tutorial

![circuitscape-tutorial](https://user-images.githubusercontent.com/50297074/137480883-c54fc4d2-cfbf-4eaf-9f09-5fb6ba89179a.png)

This repository is produced within the IAAC Internet of Cities studio 2021 - Circuitscape tutorial.
The tutorial aims to achieve **draft** ecological connectivity models based on the [Corine Land Cover](https://land.copernicus.eu/pan-european/corine-land-cover) raster layer .

Find more info at http://www.iaacblog.com/programs/mact-2122-internet-of-cities/

## Requirements
- [QGIS](https://qgis.org/en/site/forusers/download.html) (with GRASS)
- [Circuitscape](https://circuitscape.org/downloads/) (v4.0.5)

## To run the simulation
- import CLC
- clip CLC on analysis area
- check the CLC_to_Resistance values 
- r.reclass the CLC with CLC_to_Resistance values -> Resistance
- r.reclass the CLC with * = NULL -> Empty
- draw locations or patches
- check their $id property
- Rasterize with attribute (Empty + locations$id) -> Focals
- export Resistance and Focals as asc 
- run Circuitscape with Resistance.asc and Focals.asc
