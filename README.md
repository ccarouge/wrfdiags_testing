# wrfdiags_testing

This repository contains code to check if the CCRC additional diagnostics are correct.

## Diagnostics description
The diagnostics are to output the maximum average wind speed and/or precipitation rate over a given period (typically daily). The averaging periods are 5min, 10min, 20min, 30min and 60min.
The average rates are calculated for each selected window starting at each time step. The diagnostics also give the time of the maximum as the time at the end of the averaging window containing the maximum rate.

## Validation description
The code in validate_wrfdly.ipynb calculates the diagnostics for the 5min averaging window and an hourly output frequency for the wind speed.

### Data requirements
As inputs you need:
* wrfout file with outputs at each timestep over several hours
* wrfdly file with the 5min average outputs for wind with an output frequency of 1 hour.
