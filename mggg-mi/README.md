# pdv-mi


Partner Data Validation for Michigan. Data Partner: MGGG

**Raw from source:**

Precinct and congressional district shapefiles: State of Michigan GIS Open Data Portal

http://gis-michigan.opendata.arcgis.com/datasets/2016-voting-precincts 

file: 2016_Voting_Precincts-shp.zip

To get data: Download > Shapefile

Block-level demographic data: MGGG states on Github (https://github.com/mggg-states/MI-shapefiles) that they used IPUMS NHGIS data
https://www.nhgis.org/
file: nhgis0001_csv.zip,

However, the RDH later learned that all of the data is from the Census, so we used extracted the data using the Census API, as can be seen in the code IN[2].

State house and Senate districts: US Census Bureau’s TIGER/Line Program
https://www.census.gov/cgi-bin/geo/shapefiles/index.php

files: tl_2011_26_sldl.zip and tl_2011_26_sldu.zip

Select year: 2011 

Select a layer type: State Legislative Districts

Select a state (upper and lower chamber): Michigan

2016 precinct-level presidential election data: MIT Elections Data and Science Lab
MGGG Link: https://electionlab.mit.edu/

Direct data set link: https://dataverse.harvard.edu/dataset.xhtml?persistentId=doi:10.7910/DVN/LYWX3D

file: 2016-precinct-president.csv for 2016 presidential election precinct-level results

**File Processing:**

MGGG File: https://github.com/mggg-states/MI-shapefiles

Processing and Validation Steps: mggg_mi_replication.ipynb

Note / Methodology: Comments on mggg_mi_replication.ipynb

