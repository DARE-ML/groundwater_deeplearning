# groundwater_deeplearning
Groundwater prediction using deep learning models

## Objective
The objective of this code repository is to provide the source code for analysis done in **Deep learning for analysis of ground-water level via stream-flow and precipitation**, to improve the transparency and enable reproducability of the results and further discussions found in the paper.

## Input data format
The data used in the analysis can be found in the data folder, and the models can be found under jupyter notebook: modelling_ver.ipynb

### Borehole data
Borehole data from boreholes 17-22 is provided in 15 minute intervals ranging from 2013 to 2020. The data provided includes the groundwater depth in metres with respect to the Australian Height Datum (mAHD)

The files provided are in a CSV format, and can be identified via the BH prefix. 

### Borehole details
Specifics about the boreholes, including location, depth and screen radius (both in mAHD) can be found in _Middle Creek bore details.xlsx_. 

### Weather station and surface measurements
Finally, weather station data used for this analysis can be found in _Middle Creek weather station.zip_, which includes rainfall (in mm). The streamflow data can be found in _Middle Creek surface.csv_, using the mAHD data for Stilling Well

# Libraries used

Library  | Comments
------------- | -------------
numPy | Standard vector and matrix processing package 
pandas | Data analysis and data manipulation tool 
matplotlib | Used in visualisations of data and results 
tensorflow | Primary source of neural network architecture 
sklearn | Supplementary tools for metrics and evaluation 


### Outputs
Groundwater level, along with rainfll and streamflow for borehole 19
![BH_19_graphs](https://github.com/DARE-ML/groundwater_deeplearning/assets/67773048/3d090e55-9732-4953-9139-27cecfcec82b)

Groundwater model using streamflow only for borehole 17
![BH_17_across_architecture](https://github.com/DARE-ML/groundwater_deeplearning/assets/67773048/18b82cc2-1818-4fbd-8cd4-80c0b00f755d)

Groundwater model using rainfall only for borehole 17
![BH_17_rainfall_across_architecture](https://github.com/DARE-ML/groundwater_deeplearning/assets/67773048/70899759-bb56-4f89-9e52-88e90d6ea734)
