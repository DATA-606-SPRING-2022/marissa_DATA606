# Population Density Influences House Purchases Post-COVID-19

## Introduction
Over the past decade, US home prices have experience steady growth. Location has been the chief criteria dictating the price and the potential buyer, but where is the location? After the pandemic, has the requirements for the property location changed. <br><br> 
Since March 2020, when COVID-19 virus has raged through the United States and around the world, this deadly virus had left a trail of numerous deaths and lingering effects of illnesses. To contain the spread of COVID-19, our way of life took a drastic turn. Physical presence at and long commute to work have been delegated to remote attendance in a part of the dwelling. A warm hug or a firm handshake have been replaced with six feet distance or a quick fist bump. Now, it seems the period of endemic is at hand. The luxury of working remotely is a possibility. Working from a far distance is not a barrier as long as internet infrastructure is in place. One could be in New York and be working forty hours a week in California. Once, our job dictates where one live. Now, no longer is a firm requirement. <br><br>
The location of the house is an important issue to a home developer, home buyer or seller. The home developer will plan where the community will be. The creation of the community will be based on the demand of the buyer. Being able foresee the needs of the buyers will dictate the price of the property. The more in demand the location of the property is, the higher the asking price will be.<br><br>

# Research Question(s)
Has there been a big change in the buying area after COVID? <br>
Has there been a shift from the high to low dense area after COVID?<br><br>

## Dataset
<img src = 'https://github.com/tmarissa/marissa_DATA606/blob/main/Images/Data%20Source.PNG'/><br><br>

## Unit of Analysis
- US County is the unit of analysis for this research. This unit is represented by the Federal Information Processing Standard (FIPS) code which is 5 digit code that uniquely identifies counties in the United States.
- Population and land area dataset are joined with FIPS code to use to derive the density.
- FIPS code is also used to joined the density and real estate data which are used for visualization and machine learning.<br><br>

## Variables/Measures 
- Average listing price (counties) will be used to analyze during 2016 to 2021.
- Density of the area (counties) with price per square will be used to analyze between before COVID-19 (2016 to 2019) and after COVID-19 (2020 to 2021).<br><br> 

## Techniques/Models 
- clustering will be the technique use in this project. Each cluster will be represented by a centroid (average) of similar points with continuous features. 

## Development/Applicaton of Machine Learning
- Lazy Predict will be used to analyze which machine learning model to be used. However, a correlational matrix will be graphed to show the relationship of each variable to the other. 

## Intended Outcomes
- A Top 10 County Housing Price Comparison from 2016 to 2021
- A Top 10 County List Price Comparison on a Map from 2016 to 2021
- A Top 10 County House Price Bar Chart from 2016 to 2021

Using these visualization techniques would further understand the market on the county level at different point in time.
