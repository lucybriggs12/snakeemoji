# Week 4 Check-In :snake:

# Identifying Gaps in Transit Access to Grocery Stores for LA Senior Citizens

## Roles

### Carolyn: Bus Route Data Person

-Develop map of bus stops/routes and create buffers (.25miles) around the stops

-Make some additional maps/charts that are useful for understanding density of seniors related to density of bus stops. 

### Monisha: Grocery Store Data Person

-Manage data cleaning and spatial analysis related to grocery store locations including but not limited to: finding data; cleaning data (including geocoding); developing maps and charts that shed light on locations of grocery stores and the relationship between the locations of seniors and grocery stores; creating walkshed buffers; and completing related analyses. 

-Research transit agencies that operate in LA to understand their size, service areas, etc. so that group can make a decision around which agencies to include in analysis 

### Adriana: Metro Line Data Person

-Update and refine mapping where seniors are head of households but without cars (2021 data) (do this week)

-Make chart that displays relationships between the density of seniors and density of metro stops 

-Develop map of metro stops and create buffers (.25 mi) around stops

-Look into recommended walking buffer zones for seniors

### Lucy: Basemap Person

-Develop a map of density of seniors by block group

-Map the zones of Metro Micro access

-Make a chart showing the block groups/ neighborhoods most densely populated with seniors


## Status update

-Working together well but feeling a little lack of direction still

-Weekly group meetings have been working well

-Starting some big picture/step-by-step project planning that has been helpful

-Spending a lot of time self-teaching, sometimes it feels like the order of what we are learning in class doesn’t always align with the order we need to do things for the project

-Feeling a little lost sometimes in class, things are moving quickly


## Data update 

### [Grocery Stores](https://data.lacity.org/Administration-Finance/Grocery-Stores/g986-7yf9) 

-We first tried to use a dataset on the City of LA data portal for  “all active businesses currently registered with the Office of Finance” tagged as grocery stores. The only complete location info in this dataset is addresses and we need coordinates to map the data. We have succeeded in geocoding some addresses, but ~15% did not get a match. More critically, this dataset is not geographically complete, so will not be usable unless we restrict our analysis to a small number of neighborhoods. 

-We are trying to work with a dataset on the [USDA containing SNAP authorized retailer locations](https://usda-fns.hub.arcgis.com/datasets/USDA-FNS::snap-store-locations/explore?location=14.098906%2C-14.634785%2C2.79). This dataset was easy to map. However, we will have to do substantial cleaning to parse this down to locations that provide meaningful access to groceries (because many other locations like gas station convenient stores are also authorized SNAP retailers)

### Bus Lines and Stops

[LA Metro](https://developer.metro.net/gis-data/)

We were able to create maps of Metro Bus Stops and Routes in the City of LA, and layer them on top of a map of population density of seniors by census block group. This process will need to be repeated with data from other transit agencies.

[LADOT - Dash](https://catalog.data.gov/dataset/ladot-dash-and-commuter-express-routes-and-stops)

[Big Blue Bus](http://gtfs.bigbluebus.com/)

Potential other transit agencies (Long Beach Transit, Culver City Bus, etc)

### [Metro Lines and Stops](https://developer.metro.net/gis-data/)

We were able to create a map of metro stops in the city of LA . This will be overlaid with the map of population density of seniors, location of grocery stores, and eventually stops will also have a .25 mile buffer around stops to show walkshed. 

### [Age: Density of Seniors](https://www.socialexplorer.com/reports/socialexplorer/en/report/0cc0f56c-9d1c-11ed-be9e-e30303f780e8)

Using the geographic boundaries and areas, we were able to create a map of population density of seniors by census block group. We will use this map to potentially narrow down to a few neighborhoods to focus on. 

### [Metro-Micro Zones](https://micro.metro.net/)

The zones had to be downloaded as individual KML files, but were combined and mapped in Jupyter. We will use the Metro Micro zones to potentially narrow our scope and focus on a few neighborhoods. We hope to find gaps and provide recommendations for an additional metro micro zone. 


## Concerns

### Major concerns

-What are the expectations for the midterm? How far along should we be in the project by then?

-Will we get feedback on our project proposal? Is this project about the right size/complexity?

-What format will our final deliverable take, and will we get guidance on how to use necessary tools/programs?

### Minor concerns

-LA Office of Finance active registered business data is missing coordinates for a substantial number of grocery stores and we are having a hard time using Python successfully geocode all addresses.

-There are around 40 transit agencies that operate bus service in LA County (and service often runs into the City of LA). This is likely too many agencies to work with, and smaller transit agencies generally do not publish data in easily usable formats. We will likely start with the three agencies that run the most service in the city (Metro, LADOT, and Big Blue Bus) but would prefer to find a feasible way to include all transit agencies. 

-We have to select a buffer distance to use for walkability (to bus stops and to grocery stores by direct walking access.)

-We need a better way to manage divergent branches in Github- Chris linked to some tutorials but still a bit confused 

-We need to learn various geoprocessing skills (e.g. buffers) to make progress on our project. 

