## Updated Proposal for Transit Gaps: Senior Access to Fresh and Healthy Food 
<b>Group Members:</b> Lucy Briggs, Adriana Ochoa, Carolyn Pugh, and Monisha Reginald

### Research Question
We will explore gaps in access to grocery stores for seniors living in the City of LA, with a particular focus on access by non-automobile modes (e.g., walking and public transit). We will measure grocery store access at the census block group level with indicators such as:
* The average distance to a grocery store 
* The percentage of residents who live within walking distance of a grocery store
* The percentage of residents who have a direct public transit connection to the nearest grocery store
* Whether or not a census block group is in an area served by the existing Metro Micro Program 

We will then use American Community Survey data on age and car ownership by census block group to explore questions such as:
* How does access differ for seniors and seniors who do not have a vehicle (in comparison to the general population)?
* How do census block groups with higher percentages of older residents compare to the rest of the city?
* Which neighborhoods have the highest number of seniors who currently cannot walk or take a direct transit route to a grocery store?

We will begin by calculating indicators for each block group by using its centroid. If possible, we will increase the precision of our calculations by using proportional allocation of census block group population data and/or using zoning data to identify a more representative point than the block group’s centroid.
### Why This Matters
Our analysis could help identify places where additional transit options are needed to increase equitable access to grocery stores through new Metro Micro services areas or additional bus routes. As the population of seniors in Los Angeles is rapidly increasing, it is becoming increasingly vital to provide mobility access for seniors that accounts for the unique barriers to accessing existing transportation systems that older adults experience.
### Spatial & Temporal Scope
* Spatially, we will focus on analysis on the City of Los Angeles. We chose to focus on the City (rather than the County) so that we can limit the number of public transit agencies that we must include in our analysis. We will use census block groups due to the small scale of our analyses concerning walkability. 
* Our analysis concerns the current state of grocery store access in Los Angeles so that we can make recommendations for new transit services that would supplement the existing system. Due to this, we will use the most recently available demographic data from the American Community Survey (2021 5-Year Estimates) as well as other up-to-date datasets. Where possible, we will use APIs to access data that may change over the course of the quarter (e.g., the locations of grocery stores) to ensure updated analyses. 
### Data Sources
* Grocery Store Locations: 
    * [USDA SNAP Authorized Retailer Locations](https://usda-fns.hub.arcgis.com/datasets/USDA-FNS::snap-store-locations/)
* Metro-Micro Zones
    * [LA Metro](https://micro.metro.net/)
* Bus Lines and Stops:
    * [LA Metro](https://developer.metro.net/gis-data/)
    * [LADOT](https://catalog.data.gov/dataset/ladot-dash-and-commuter-express-routes-and-stops)
    * [Big Blue Bus](http://gtfs.bigbluebus.com/)
* Metro Lines and Stops:
    * [LA Metro](https://developer.metro.net/gis-data/) 
* Census Data:
    * Age: [American Community Survey](https://www.socialexplorer.com/reports/socialexplorer/en/report/0cc0f56c-9d1c-11ed-be9e-e30303f780e8)
    * Car Ownership: American Community Survey accessed through [Social Explorer](https://www.socialexplorer.com/tables/ACS2021_5yr/R13284517) and [Census API](https://data.census.gov/table?q=B25045:+TENURE+BY+VEHICLES+AVAILABLE+BY+AGE+OF+HOUSEHOLDER&g=0100000US_1600000US0644000&tid=ACSDT1Y2021.B25045)
* Geographic Boundaries:
    * [City Boundary from LA GeoHub](https://geohub.lacity.org/datasets/city-boundary/explore?location=34.019779%2C-118.412043%2C10.96)
    * [LA Times Neighborhood Boundaries](https://geohub.lacity.org/datasets/d6c55385a0e749519f238b77135eafac_0/)
    * [Block Group Boundaries from LA GeoHub](https://geohub.lacity.org/datasets/lacounty::census-block-groups-2020/explore)
### Analysis & Visualizations
This project will analyze access to grocery stores by walking or public transportation in areas with high concentrations of senior citizens. Our visualizations will include maps of grocery store locations and residential areas that are within a walkable distance to a grocery store. We will also produce overlay maps with transit networks and census data depicting where seniors live. 
### Conclusion & Expectations 
We hope to understand the disparities in access to grocery stores by non-automobile modes for seniors. Understanding disparities in service can help to inform service expansions through traditional fixed-route transit or innovative programs like Metro Micro to ensure equitable access to mobility for all residents of Los Angeles.