**Freshest**  v1.3.0 - 2016-10-04

This web application for helping people in Chicago or even other places to find relatively cheap, fresh and accesible vegetables.  
Keywords: fresh vegetables, price, weather, local produce


**v1.3.0 Update**  

New layout was applied to the original website. As user need to know direct information of freshness. We use an evaluation standard of freshness for certain market or store based on multiple information datasets. This can provide additional information for the user to compare different places to go.
More functions are added in the map system. User can choose to switch to their current location by clicking on the blue button on the top-left corner. So they can do further searching on markets with vegetables nearby. Bugs are fixed. User can search for places with vegetables directly so that user can find out where to have vegetables. Also seasonal chart can provide the freshest vegetables to have in certain season (month).      
A line chart of vegetable price changes is added. User can mouse over different point to see the vegetable price changing rate of different year. It can be positive (price increases) or negative (price decreases). So that user will have an insight of food price changing trend and know approximately what year might have relatively cheaper vegetables.  
Climate/weather information will be applied in Chicago region as a form of heatmap (colored circles on map). So that user can see temperature condition which potentially affects the freshness of food. (e.g.: overly hot weather will lead to shorter preserving time of vegetables)
 

Demo website: http://web.ics.purdue.edu/~gao338/freshest/home.html

**Description**

* Datasets  
Most datasets come from data.gov, some other functions are included as well.  
(More datasets will be added later. Existing datasets maybe modified later.)  
  * Climate Data Online (http://www.ncdc.noaa.gov/cdo-web/datasets)  
  Daily Summaries for Indina From 01/01/2008 to 12/31/2010  
  Columns used: Preciptation, Water, Winds, Maximum temperature, Minimum temperature, Weather type (sunny, snow, rain...etc)

  * Price of Local Vegetables  
  local price of vegetables will be obtained from http://catalog.data.gov/dataset/   
  (Still on process to find a more complete dataset of local price foe vegetables)  
  This dataset will give information of location of market, price for certain vegetables

  * Seasonality Chart (https://www.cityofchicago.org/city/en/depts/dca/supp_info/farmers_market0.html)  
  se the seasonality chart below to find out when your favorite fruits and vegetables are ripe and ready to eat!.
  Column used: names, all months


* Map View  
  * Initialized Map View will focus on Chicago, as they are our main users for now.  
  * Market location will be marked on map. Name and detailed information will expand in tooltip after clicking
  * When move the mouse over a target, the current mark will be highlighted and show name of the market.
  * There would be transparency change of certain location based on the climate data to show freshness of vegetables.
  * Map is added with function showing market location and information. Map is customized with different style.  
  * User can search for any markets or grocery stores by keywords. All search results can be extended to larger or smaller scale when user try to zoom in or zoom out. They can also customize the search. An autocomplete function for the search box was applied. User can choose to switch to their current location by clicking on the blue button on the top-left corner. So they can do further searching on markets with vegetables nearby.  

* Data Visualization  
  * We use chart visualization from D3.js. We create pie for comparison of vegetables from different season. When mouse over a month, the chart will show vegetables available. Also we have a line chart for changes in food price for consumer. This is for having an insight of food price changes. So user can have a sense of the food price trend.  
  * A new seasonal chart for vegetables and fruits is added. It shows specific type of vegetable and fruits available at certain month. 


* Interaction Form
  * The interaction of the system will mostly be clicking and showing information.
  * Information input: User need to give keywords on search bar or click on specific marker. Use slidebar will give input of selected year or month.
  * Information output: The marker of each market will give information like weblink, avalable product or freshness evaluation. These will be in a form of charts rather than plain text.
  * Operation option: User can search vegetables or specific market.
  * Interaction with Map: 1. User can zoom in/out on google map, check location of markets, click on highighted marker to see market weblink or avalable products. This can coordinate with other charts on dashboard as well.
  * interaction with data visualization: user can mouse over the searson chart to see monthly change of available vegetables. User can also mouse over line chart to see the vegetable price changes (increase/decrease) details.

**Build up Information**  
This project uses HTMl/CSS/Javascript. Other decendencies like python will probably be used as well in terms pf pre-processing data. README file will be updated at different phases with detailed description of the project.

**Test**  
The project will be tested on Chrome.
