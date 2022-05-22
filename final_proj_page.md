Project Description

One major issue that the world is grappling with is Environmental Injustices. Environmental injustices occur when a particular group faces an unequal distribution of negative impacts based on demographics, such as race. Historically around the US and even around the world, people of color face the greatest environmental injustices, and Baltimore City is no different. In Baltimore City, a large number of people take public transportation, and often time riders will take the bus to get to where they need to be. One aspect of riding a bus is waiting at a bus stop, and not every bus stop is the same, some have shelters, others are just a sign on the side of the road. Of those stops that do not have a shelter, trees can often time act as a shelter, provide shade, provide some protection from the elements, lower the urban heat island effect, and even beautify the city. To determine if there is a correlation to bus stops that do not have shelters and tree cover in Baltimore City an R-analysis will be undertaken. As well as looking at the relationship to bus stops and tree cover, census data will be used to see if there is a correlation to the lack of shelter and trees at bus stops is correlated to income and race. 

Research Question: 

How are bus stops without shelter from the Maryland Transit Agency distributed across Baltimore City, and is there a correlation to Race, Income, and tree cover?


Data:
	- MDOT MTA Bus Stops - Source: Maryland Open Data Portal
	- Demographic Data (Median Household Income, Race) - Source: United States Census Bureau 
	- Baltimore City Tree Cover - Source: Provided from a previous lab

Methods:

To answer the research question, a spatial analysis will be undertaken. The first step was to filter all of the MDOT MTA bus stops down to only those within Baltimore City. Then those bus stops were filtered further to include those that do not have a shelter, the sheltered bus stops were used to compare to the unsheltered bus-stops. The next step was collecting data from the census bureau for median household income and race by census tract. Once all the data was gathered and cleaned up the analysis began. First, each bus stop, both sheltered and unsheltered, were buffered out to 250m, because only what was immediately around the bus stop was being observed. Once I had the buffers, I extracted the tree cover sum from the tree canopy raster data for each bus stop buffer. Then visuals were created, first census data was visualized as 6 classes going from low to high. Second, each bus stop canopy cover was visualized as 6 classes going from low canopy cover to high canopy cover. 

The other aspect of the analysis was to see if there was an unequal distribution of sheltered bus stops. To do this each census variable was visualized as before, and then I created a tessellation using hexagons to show the density of sheltered bus stop points, and overlayed the tessellation onto each of the census variables. 

Results/Conclusion:
The following map shows Median Household Income for Baltiore City and buffered MTA Bus Stops Tree Cover.
<img src= "images/Screen%20Shot%202022-05-21%20at%2010.25.48%20PM.png"/>

This map shows White Population for Baltiore City and buffered MTA Bus Stops Tree Cover.
<img src= "images/Screen%20Shot%202022-05-21%20at%2010.26.07%20PM.png"/>

This map shows Black Population for Baltiore City and buffered MTA Bus Stops Tree Cover. 
<img src= "images/Screen%20Shot%202022-05-21%20at%2010.26.19%20PM.png">

This map shows Native Population for Baltiore City and buffered MTA Bus Stops Tree Cover.
<img src= "images/Screen%20Shot%202022-05-21%20at%2010.26.31%20PM.png"/>

This map shows Asian Population for Baltiore City and buffered MTA Bus Stops Tree Cover.
<img src= "images/Screen%20Shot%202022-05-21%20at%2010.26.44%20PM.png"/>

This map shows Hispanic Population for Baltiore City and buffered MTA Bus Stops Tree Cover.
<img src= "images/Screen%20Shot%202022-05-21%20at%2010.26.53%20PM.png"/>

Lastly, this map shows the distribution of sheltered MTA bus stops across Baltimore City, overlayed onto each census data variable. 
<img src= "images/Screen%20Shot%202022-05-21%20at%2010.27.02%20PM.png"/>

After performing this analysis, there were two key findings, one is that bus stops that are sheltered are more likely to be in areas that are white and wealthy. Two of the unsheltered bus stops, the highest canopy coverage were in the areas that were of higher income and whiter. These findings reinforce the need for environmental justice and to drive more tree planting and maintenance in areas that are non-white and of lower income. 
