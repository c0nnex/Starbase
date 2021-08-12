# Buffalo Generator and Fuel Calc

This script will change the default Generator script to
* Allowing to set a Minimum Generator Rate
* Calculating percentage of fuel rods and propellant remaining

With default configuration the Mininglasers will not drain batteries at a Generator-Rate of 40%

Generators need approx 1s per Percent to Spool up, so 40 seconds from 0 to 40%. (Just the time approach needs)

## How to install

* Create a Field "MinGen" in the MemoryChip (bottom right rack) with value "0".
Will be used in other scripts to set a minimum generator rate.
* Loop through all 16 Fuel Chambers and rename "FuelChamberFuel" to "FR#" (replace # by number 1-16) 
* Change "Fuel_Rods" Display:
  * Change "PanelMaxValue" to "100"
  * Change "PanelVariableResolution" to "0.01"
* Change Propellant Display:
  * Rename first field to "Prop_Percent"
  * Change PanelMaxValue to 100
  * Change PanelVariableResolution to 0.01
* Exchange Generator Script by GenAndFuel.yolol (Middle Chip, first Right Rack)
