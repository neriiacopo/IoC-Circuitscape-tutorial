Tutorial - Circuitscape

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
