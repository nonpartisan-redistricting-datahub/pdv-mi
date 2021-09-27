# vest-mi-2020

Our final validation report for this dataset is available [here](https://redistrictingdatahub.org/dataset/vest-2020-michigan-precinct-boundaries-and-election-results-shapefile/).

We do not have the raw data sources available on this Github due to file constraints, but we are happy to share them if needed. 

Please reach out to info@redistrictingdatahub.org to reach our support team if you have any questions.

## Raw from source:

- File: VEST MI 2020 file
   - Date accessed: 07/26/2021
   - Link: https://dataverse.harvard.edu/file.xhtml?fileId=4863165&version=20.0
- File: VEST documentation file, 2020
   - Date accessed: 07/26/2021
   - Link: https://dataverse.harvard.edu/file.xhtml?fileId=4931790&version=20.0
- File: Election Results, SOS 2020
   - Date accessed: 07/26/2021
   - Link: https://miboecfr.nictusa.com/cgi-bin/cfr/precinct_srch.cgi
   - Note: Make sure you have "All Counties" selected, click "Search" and then click "HERE".
- File: Precinct Shapefile, 2020 
   - Date accessed: 5/26/2021
   - Link: https://gis-michigan.opendata.arcgis.com/datasets/49eb37d0a4294924bf8ef5ffe0eac47e_6/explore
   - Note: There is a download button on the left side of the screen.
- File: AVCB Mapping 
   - Date accessed: 08/23/2021
   - Link: https://github.com/openelections/openelections-sources-mi/blob/master/2020/Detroit%20AVCBs%20by%20precinct%20(Nov.%202020).xlsx
- File: Census Geocodes, 2020 
   - Date accessed: 08/23/2021
   - Link: https://www.census.gov/geographies/reference-files/2020/demo/popest/2020-fips.html
- File: MI County Shapefile
   - Date accessed: 09/27/2021
   - Link: https://gis-michigan.opendata.arcgis.com/datasets/67a8ff23b5f54f15b7133b8c30981441/explore?location=44.916500%2C-86.594000%2C6.81
   - Note: Didn't use the precinct shapefile for this, because VEST mentions that that file does not always split precincts across counties correctly.


## File processing:

`vest-mi-2020-validation.ipynb` is the script that is the basis of the validation report
