# Remote Sensing and Durian Cultivation
NASA Space Apps Challenge 2024  
Team Grow from Singapore

## Presentation Slides
https://docs.google.com/presentation/d/1rW3BJv7LVbnAB3SYe2VXp8pb-IIRhqz9v-cKkGGlLXg/edit?usp=sharing

## NASA Data Resources

### Agricultural and Water Resources
https://www.earthdata.nasa.gov/learn/pathfinders/agricultural-and-water-resources-data-pathfinder

#### Physical Geography / Topology
The ASTER instrument on the terra satellite provides topograhical data to 15m resolution.
https://www.earthdata.nasa.gov/sensors/aster

Here is a link to ASTER data around the Raub, Pahang, Malaysia durian growing area.
https://search.earthdata.nasa.gov/search/granules?portal=idn&p=C2439422590-LPCLOUD&pg[0][v]=f&pg[0][bo]=true&pg[0][oo]=true&pg[0][gsk]=-start_date&g=G2439801591-LPCLOUD&sb[0]=101.39941%2C3.47693%2C102.375%2C4.14084&fi=ASTER&tl=1728121636.043!3!!&lat=3.6192491017884407&long=100.05908203125&zoom=7

This is a sample image showing the hilly high draining topography favourable for durian growth.

![Raub area Digital Elevation Model](/images/raub-dem.png)

#### Gobal Emissivity.
ASTER sourced emissivity data is available:
https://search.earthdata.nasa.gov/search/granules?p=C2763266348-LPCLOUD&pg[0][v]=f&pg[0][gsk]=-start_date&g=G2817962046-LPCLOUD&sb[0]=101.51367%2C3.46833%2C102.43213%2C3.97396&fi=ASTER&gdf=HDF&tl=1728126360.354!3!!

It is in hdf-eos version 5 format.

There is a python library available to work with hdf5. Get it here:
https://www.hdfeos.org/software/h5py.php

This tool should be able to extract multi-spectral data from the ASTER data set:
"The Advanced Spaceborne Thermal Emission and Reflection Radiometer (ASTER) obtains high-resolution images of Earth in 14 different wavelengths of the electromagnetic spectrum, ranging from visible to thermal infrared light. Scientists use ASTER data to create detailed maps of land surface temperature, emissivity, reflectance, and elevation. ASTER is the only high spatial resolution instrument aboard the Terra satellite. "

There is a HDF viewer available from:
https://github.com/HDFGroup/hdfview/releases/tag/v3.3.2

##### NDVI Normalized Difference Vegetation Index
This data set looks promising!

![ndvi](/images/raub-ndvi.png)


#### Soil Moisture
The SMAP (Soil Moisture Active Passive) satellite provide soil moisture date at 9km resolution.

Here NASA worldview link for soil moisture in the Raub region on 2023-Aug-05 (Durian Harvest Season).
https://worldview.earthdata.nasa.gov/?v=97.8519037473553,1.8593583483940634,104.38676061836128,5.147208211618951&ici=3&icd=1&l=Reference_Labels_15m,Reference_Features_15m,Coastlines_15m,SMAP_L2_Passive_Enhanced_Day_Soil_Moisture_Option1,ASTER_GDEM_Color_Shaded_Relief(hidden),MODIS_Terra_CorrectedReflectance_TrueColor(hidden)&lg=false&t=2023-08-05-T12%3A00%3A00Z

And this is image snapshot.
Yellow is dry and Blue is wet.

![raub soil moisture snapshot](/images/raub-smap.png)

## Google Earth data

Google Earth (Cloud-free) data on the Raub region.
https://earth.google.com/web/search/raub+pahang/@3.84068769,101.85897802,144.83445023a,519.37912909d,35y,0h,0t,0r/data=CnoaTBJGCiUweDMxY2JlZjlmNGZlZTM4YWY6MHhkNjY5OGUzOWNmNjE5YTBlGcKiIk4nWQ5AIYd9TLXgdllAKgtyYXViIHBhaGFuZxgBIAEiJgokCdf6EVGrrxVAEQV5zacdbBRAGXSCBoCKOVlAISoOAtMqEVlAQgIIAToDCgEwSg0I____________ARAA

The image snapshot below clearly shows dicernible patterns for durian plantations.

![durian plantation snaphot](/images/raub-google-earth.png)

