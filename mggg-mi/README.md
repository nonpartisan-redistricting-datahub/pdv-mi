# pdv-mi

Partner Data Validation for Michigan. Data Partner: MGGG

## Raw from source

### Precinct and congressional district shapefiles
State of Michigan GIS Open Data Portal
http://gis-michigan.opendata.arcgis.com/datasets/2016-voting-precincts 

file: `2016_Voting_Precincts-shp.zip`
To get data: Download > Shapefile
Note: had some issues downloading the CD shapefiles from here, so used TIGER instead and got the same results. 

### Block-level demographic data
MGGG states on Github (https://github.com/mggg-states/MI-shapefiles) that they used IPUMS NHGIS data
https://www.nhgis.org/
file: `nhgis0001_csv.zip`

However, the RDH later learned that all of the data is from the Census, so we used extracted the data using the Census API.

### State House, State Senate, Congressional districts
US Census Bureau’s TIGER/Line Program
https://www.census.gov/cgi-bin/geo/shapefiles/index.php

files: `tl_2013_26_sldl.zip` and `tl_2013_26_sldu.zip`

Select year: 2013 
Select a layer type: State Legislative Districts
Select a state (upper and lower chamber): Michigan

files: `tl_2013_us_cd11.zip`

Select year: 2013 
Select a layer type: Congressional Districts

Note: first we tried to use 2011 legislative but we have to use post-2012 boundaries because redistricting was in 2012. 

### 2016 precinct-level presidential election data
MIT Elections Data and Science Lab
MGGG Link: https://electionlab.mit.edu/
Direct data set link: https://dataverse.harvard.edu/dataset.xhtml?persistentId=doi:10.7910/DVN/LYWX3D

file: `2016-precinct-president.csv` for 2016 presidential election precinct-level results

## File Processing

MGGG File: https://github.com/mggg-states/MI-shapefiles

Processing and Validation Steps: `mggg_mi_replication_for_report.ipynb`
(`mggg_mi_replication.ipynb` was the first draft before writing the report)

Note / Methodology: Comments on `mggg_mi_replication_for_report.ipynb`

