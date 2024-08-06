# LS123-Data-Prediction-Law
LS123 SU24


# readme

1. use merging.ipynb : For the call for service data, I divided into whether it was an intersection or not, address number and street name with a block address. In the case of alcohol, business and store names were matched by tasks such as removing symbols from the store name and removing spaces, leaving only active ones. After that, he added to the business whether or not they sell alcohol. Here, the address was also divided into address number and street, the same as pd_calls.
2. use MERGING2.ipynb : Use the data set that combines business and alcohol obtained in No. 1 and the pdcall data set with the changed address part. The way the addresses are written in these two datasets are different, so make it same and merge them. The combined data is divided into 10000 pieces and posted on the census bureau site. Through this, lat, lon, trace code, and block code are obtained and combined.
3. Now the finished data is data_project.csv. Use this to do the modeling.



# Project question - risk of crime on certain streets near Berkeley
 
## Outcome of interest (dependent variable): risk of crime
## Independent variables/covariates/ predictors, features : proximity to police, Types of surrounding commercial facilities, population density, land type, street lighting
## Potential explanations for the association of variables : 
1.  	Areas with certain types of commercial facilities, such as bars, may experience more crime due to increased foot traffic and alcohol consumption.
2. 	Higher population density might correlate with more crime due to increased opportunity.
3. 	Streets farther from police stations may have slower response times and thus higher crime rates.
4. 	Streets with brighter lighting are expected to have less crime compared to darker streets.
5. 	Flat areas are likely to experience less crime compared to sloped areas due to better visibility and accessibility, which can aid in crime prevention.
## Possible units of analysis : individual streets in the Berkeley area
## Time period : 1 academic year ( 2023 spring, summer, fall )
## Jurisdiction : Berkeley

## Motivation
As students at UC Berkeley, the safety and well being of all students and residents in the Berkeley area is of utmost importance to us. By understanding the factors that influence crime and identifying the high risk areas in Berkeley, this research can influence local law enforcement policies, university guidelines, or even greater community initiatives. This could include strategizing and changing police patrol routes, designing safer infrastructure, and implementing college safety programs like Bear Walk. 



# Data we used

1.      Call for service : https://bpd-transparency-initiative-berkeleypd.hub.arcgis.com/datasets/3be134af40954e19a3d308779a65f175_0/explore?filters=eyJEaXNwb3NpdGlvbnMiOlsiUHJpbWFyeSBDYXNlIChDYXNlIG9yIENvbGQgVGhlZnQpIiwiSW5jaWRlbnQgUmVwb3J0Il0sIkNyZWF0ZURhdGV0aW1lIjpbMTY3MjkyOTM2OTE2NC41NiwxNzIxMDU1NjAwMDAwXX0%3D
2.     Commercial : https://data.cityofberkeley.info/Business/Business-Licenses/rwnf-bu3w/about_data
3.     census : (https://geocoding.geo.census.gov/geocoder/geographies/addressbatch?form)
4.  alcohol (Active Retail Licenses, Berkeley): https://www.abc.ca.gov/licensing/licensing-reports/adhoc-report/?RPTTYPE=9&CITY=BERKELEY



