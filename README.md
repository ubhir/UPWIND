# UPWIND

## McMaster University - McMapster 

### ECCE App Challenge 2019

### Team Members
Yorgan Pitt, Edward Seh-Taylor, Sean Leipe, Raj Ubhi 

## Mission Statement 

**Upwind** aims to highlight the potential of rooftop wind power in improving the sustainability of urban power generation in Vancouver, British Columbia.

The accessibility of reliable and renewable energy is a key component in developing sustainable urban communities. To date, only 17.4% of the Canadian national energy supply is derived from renewable sources [1]. Despite wind power surging forward as one of the fastest growing energy sources worldwide, only 5% of electricity generation in Canada comes from wind. Between 2013 to 2017 the Canadian government invested $13.7 billion into the development of wind-powered energy generation [1]. One less-explored facet of wind power comes from small, rooftop-mounted turbines.

The city of Vancouver continues to grow and develop with, with $5.1 billion dollars of building permits issued in 2018 alone. Currently, a large portion of Vancouver’s energy stems from natural gas and hydropower. The city has set a target of achieving 100% renewable energy consumption by the year 2050 [2]. With a focus on generating clean energy to power their urban development, Vancouver is a potential site for urban wind power generation. 

Vertical axis wind turbines (VAWTs) have been found to be advantageous to traditional horizontal axis turbines (HAWTs) in several aspects [3]. The design of vertical turbines compensates for some of the shortcomings found in traditional wind power technologies, as they can be placed very close to one another with minimal or no loss of efficiency [4]. Vertical turbines have also been shown to work better than their horizontal counterparts in sub-optimal wind climates, such as rooftops. 

## App Characteristics

3D building multipatches were created by extruding building footprints from Vancouver’s Open Data portal, according to their provided roof heights. Several important wind energy attributes were calculated for each of these buildings based on numerical modeling simulations found in the Canadian Wind Atlas. These numerical models were  applied to power curves representative of modern commercial VAWT systems. Considering the wide variability of different models of VAWTs, we estimated power generation from an generalized wind turbine model. 

The properties for our theoretical VAWT model were derived from the average properties of several small commercially available VAWT systems, with the diameter of the turbine was set to 2.5m. The Wind cut-in was set to 2m/s and the rated windspeed was set 12m/s. The rated power of our turbines was set 1000w, approximately the industry average. By modifying the power generation equation acquired from Natural Resources Canada, the maximum potential wind power output was calculated with:

*Power (kWh)=((100*(WindSpeed)-200)*0.031536)/0.0036*
 
**Analyzing Existing Buildings**

For each neighbourhood in Vancouver we have a 3D web scene containing buildings, classified by zoning category.

Several energy-related attributes have been calculated for every building in each neighbourhood, based on numerical modeling simulations taken from the Canadian Wind Atlas at 30m, 50m, and 80m above sea level. The roof area of a building allows us to calculate how many turbines can be theoretically mounted on it, based on their required separation distance for maximum efficiency. By referencing the Wind Atlas projections based on each building’s absolute height above ground,  the maximum yearly power output for each individual turbine has been calculated. By multiplying this by the maximum number of turbines the building can hold, we obtain the maximum potential wind power for this building in kWh.

Average energy production for several types of households in British Columbia was obtained from Statistics Canada [5]. By comparing the maximum potential wind power output to the given value from StatsCan, the app can calculate the percentage of total energy saved per household. Due to the extreme variability in energy consumption of non-residential buildings, consumption and potential saved energy were not calculated for these.
 
**Exploring Future Potential**

The interactive portion of our app lets the user evaluate wind potential at any site in Vancouver using a heavily configured version of the Smart Editor Widget.

This gives the mean annual speed and potential energy per turbine in kWh for heights of 30m, 50m, and +80m.
