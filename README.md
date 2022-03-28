# Impact of COVID-19 on the US Housing Market

## Introduction
Over the past decade, US home prices have experience steady growth. Location has been the chief criteria dictating the price and the potential buyer, but where is the location? After the pandemic, has the requirements for the property location changed. <br><br> 
Since March 2020, when COVID-19 virus has raged through the United States and around the world, this deadly virus had left a trail of numerous deaths and lingering effects of illnesses. To contain the spread of COVID-19, our way of life took a drastic turn. Physical presence at and long commute to work have been delegated to remote attendance in a part of the dwelling. A warm hug or a firm handshake have been replaced with six feet distance or a quick fist bump. Now, it seems the period of endemic is at hand. The luxury of working remotely is a possibility. Working from a far distance is not a barrier as long as internet infrastructure is in place. One could be in New York and be working forty hours a week in California. Once, our job dictates where one live which no longer is. <br><br>
The location of the house is an important issue to a home developer, home buyer or seller. The home developer will plan where the community will be. The creation of the community will be based on the demand of the buyer. Being able foresee the needs of the buyers will dictate the price of the property. The more in demand the location of the property is the better the asking price.<br><br>

## Research Question(s)
Has there been a change in house prices since COVID-19? <br>
Has there been a change in in-demand house location since COVID-19?<br>
Has there been a change in buyers' house buying criteria since COVID-19? <br><br>

## Dataset
<img src = 'https://github.com/tmarissa/marissa_DATA606/blob/main/Images/Data%20Source.PNG'/><br><br>

## Unit of Analysis
- US County is the unit of analysis for this research. This unit is represented by the Federal Information Processing Standard (FIPS) code which is 5 digit code that uniquely identifies counties in the United States.
- Population and land area dataset are joined with FIPS code to use to derive the density.
- FIPS code is also used to joined the density and real estate data which are used for visualization and machine learning.<br><br>

## Variables/Measures 
- Average listing price (counties) will be used as the dependent variable and will be to analyze during 2016 to 2021.
- Density of the area (counties) with price per square will be used to analyze between before COVID-19 (2016 to 2019) and after COVID-19 (2020 to 2021).
- There will be 25 variables used as independent variables, Active Listing Count, Avg Listing Price, Avg Listing Price M/M, Avg Listing Price Y/Y, County, Date, Days on Market, Days on Market M/M, Days on Market Y/Y, Density, FIPS, Median List Price Per Sqft, Median Listing Price, Median Listing Sqft, New Listing Count, Pending Listing Count, Pending Ratio, Price Decrease Count, Price Decrease Count M/M, Price Decrease Count Y/Y, Price Increase Count, Price Increase Count M/M, Price Increase Count Y/Y, State, Total Listing Count.
- These are the links to the description of the [variables.](https://github.com/tmarissa/marissa_DATA606/blob/main/Images/Data%20Variable.PNG) <br><br>

## Techniques/Models 
- K-means will be the technique used in this project which works by selecting how many clusters, k, exist in the data. Each cluster will be represented by a centroid (average) of similar points with continuous features. Principal Component Analysis (PCA) will also be used because it help reducing the number of dimensions for the data set. This works by finding a lower dimension in the data such that the variance is maximized. <br><br> 

## Development/Applicaton of Machine Learning
- Lazy Predict will be used to analyze which machine learning model to be used. However, a correlational matrix will be graphed to show the relationship of each variable to the other.<br><br> 

## Intended Outcomes
This research intends to understand how COVID-19 change the real estate market. This can help real estate developers and local government planners in designing future housing sites.<br><br>

## Exploratory Data Analysis
### Correlational Matrix<br>
<img src = 'https://github.com/tmarissa/marissa_DATA606/blob/main/Images/Correlation%20Matrix.png'/><br>
In this matrix, the highest correlation is between average listing price and median listing price which is 83%. The second highest correlation is between average listing price yy (yearly change) and median listing price yy (yearly change) which is 64%.<br><br>

### Box Plot for Average Listing Price per State
- 2019 Box Plot<br>
<img src ="https://github.com/tmarissa/marissa_DATA606/blob/main/Images/2019%20Box%20Plot%20for%20State's%20Average%20List%20Price.PNG" /><br><br>

- 2021 Box Plot<br>
<img src ="https://github.com/tmarissa/marissa_DATA606/blob/main/Images/2021%20Box%20Plot%20for%20State's%20Average%20List%20Price.PNG"/><br><br>

There is a difference in the demand of the housing in the different states in the United States. While Hawaii has constantly has the highest listing price before and after COVID, the next highest most expensive shifts after the pandemic. In 2019, the remaining four top states were District of Columbia, Massachussetts, Rhode Island, California respectively before the pandemic. By 2021, the remaining top four states showed a change in the ranking. The District of Columbia was displaced to the third while Rhode Island became second most expensive. It is followed by Massachussets which kept its fourth placement. Lastly, California maintained its fifth placement.<br><br>

### Mapping for Average Listing Price Change (%) per State
- 2019 State Map
<img src ="https://github.com/tmarissa/marissa_DATA606/blob/main/Images/2019%20ALP%20%25:state.png" /><br><br>

- 2021 State Map
-<img src ="https://github.com/tmarissa/marissa_DATA606/blob/main/Images/2021%20ALP%20%25:state.png" /><br><br>

Comparing the 2019 and 2021 maps, the top 10 states in the United States that enjoyed high average listing price change are not consistent. However, three states are found in 2019 and 2021 top ten list. They are Idaho (41.48%), Alaska (28.40%), and South Dakota (26.32%). Here is the link to [502 States and FIPS.ipynb](https://github.com/tmarissa/marissa_DATA606/blob/main/ipynb/502%20States%20and%20FIPS.ipynb). Refer to 2.2c Consistent Top 10 Highest Price Increase (2019 and 2021) 


## K-Means Model Execution
<img src ="https://github.com/tmarissa/marissa_DATA606/blob/main/Images/2019%20FIPS%20K-Means%20Scatterplot.PNG" width='2000' /><br><br>
<img src ="https://github.com/tmarissa/marissa_DATA606/blob/main/Images/2021%20FIPS%20K-Means%20Scatterplot.PNG" width='2000'/><br><br>
<img src ="https://github.com/tmarissa/marissa_DATA606/blob/main/Images/2019%202021%20FIPS%20K-Means%20Choropleth.PNG" width='2000' /><br><br>
In 2019, the predominant brown cluster begins from Midwest region going towards East. In 2021, the cluster in the Midwest region is isolated from the other regions. The formerly brown East North Central region onward to east belongs to their own cluster.<br><br><br><br>
<img src ="https://github.com/tmarissa/marissa_DATA606/blob/main/Images/2019%20MA%20K-Means%20Scatterplot.PNG" width='2000'/><br><br>
<img src ="https://github.com/tmarissa/marissa_DATA606/blob/main/Images/2021%20MA%20K-Means%20Scatterplot.PNG" width='2000'/><br><br>
<img src ="https://github.com/tmarissa/marissa_DATA606/blob/main/Images/2019%202021%20MA%20K-Means%20Choropleth.PNG" width='2000'/><br><br>
In 2019, Berkshire and Hampshire counties belong to one cluster. Berkshire has a 139 density and 31.60 rural percentage while Hampshire has a 307 density and 21.44 rural percentage which meant Berkshire is less dense and less urban than Hampshire. In 2021, Berkshire is in its own cluster. Its average listing price rose from 631K to 975K. Hampshire clustered with Hampden. Hampden has a 570 density and 18.39 rural percentage. Both Hampshire and Worcester are more urban than Berkshire but their average listing price is around 500’s.<br>  




