# geo_scout
Mapping Scouts data to UK administrative regions.

## Prerequisites: ##
This is written and tested in Python 3.7.2.

There are several python packages that are required to be installed, including:
 * pandas
 * geopandas
 * numpy
 * folium

## Getting Started: ##
You will need to obtain the latest version of the ONS Postcode Directory. Note
that this has some open licences attached to it.

If this is not May 2018, then you will need to create another child class of
ONSData in ONS_data.py

You will need to populate the settings.json file with the appropriate file paths

### Resources: ###
######Postcode Directory:
 * Latest ONS Postcode Directory ([link](https://geoportal.statistics.gov.uk/search?collection=Dataset&sort=-modified&tags=ons%20postcode%20directory))

###### Shapefiles: ######
*Use the same boundary resolution for each of the following (BFE, BFC, BGC, BUC)* 
 * Local Authority Districts Boundaries UK BGC ([link](https://geoportal.statistics.gov.uk/search?collection=Dataset&sort=-modified&tags=bdy_lad))
 * Counties and Unitary Authorities Boundaries UK BGC ([link](https://geoportal.statistics.gov.uk/search?collection=Dataset&sort=-modified&tags=BDY_CTYUA))
 * Wards Generalised Clipped Boundaries UK ([link](https://geoportal.statistics.gov.uk/search?collection=Dataset&sort=-modified&tags=BDY_WD))
 * Westminster Parliamentary Constituencies UK BGC ([link](https://geoportal.statistics.gov.uk/search?collection=Dataset&sort=-modified&tags=BDY_PCON))
 

 * Lower Layer Super Output Areas (England & Wales) ([link](https://geoportal.statistics.gov.uk/search?collection=Dataset&sort=-modified&tags=BDY_LSOA%2CDEC_2011))
 * Middle Layer Super Output Areas (England & Wales) ([link](https://geoportal.statistics.gov.uk/search?collection=Dataset&sort=-modified&tags=BDY_MSOA))
 * Scottish Intermediate Zone Boundary ([link](https://data.gov.uk/dataset/133d4983-c57d-4ded-bc59-390c962ea280/intermediate-zone-boundaries-2011))

The Beginner's Guide to UK Geography ([link](https://geoportal.statistics.gov.uk/search?collection=Document&sort=name&tags=DOC_BGG)) can be useful as an introduction for those new to GIS.

**Notes:**
I suspect that this will generalise beyond the specific application to Scouts,
but I have not done so. I anticipate to progress to this point, but unfortunately
the code will only work out of the box with data structured as an extract of
the Scout Census.

The documentation and commenting are imperfect and being improved, and can be
found here: 

I would welcome any support, comments or guidance on my code.

*This project is licensed under the GNU License - see the LICENSE file for details*
