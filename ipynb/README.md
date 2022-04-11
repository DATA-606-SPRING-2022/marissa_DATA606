# This folder contains notebooks<br>
### 101 Population, Land Area, and Real Estate.ipynb
- get the land area dataset from US census, population dataset from USDA, real estate dataset from realtor.com
- the dataset are cleaned, merge, and saved. 
    - Population and Land Area on FIPS level saved as Pop_Land.csv
    - Population and Land Area on state level saved as State_Pop_Land.csv
    - Real Estate saved as Real_Estate.csv <br>
- Real_Estate.csv can't be found in the csv folder because it is too large to upload

### 201 Merged Land Area, Population, and Rural Percentage.ipynb 
- compute the density by diving land area to population
- scatter plots for the densities for 2019 and 2020, for States' rural percentage and rural category
- merging the land area, population and rural percentage
- saved Density.csv

### 301 Merged Density and Real Estate.ipynb
- Merged the density and real etate dataset
- Remove null values
- Show MSNO matrix
- Saved to RE_Density.csv
- RE_Density.csv can't be found in the csv folder because it is too large to upload

### 401 Box Plot, Matrix and Bar Chart.ipynb
- Correlation matrix
- Split data to 2019 and 2021
- Percentage of counties average listing price increased from 2018 to 2021
- Scatter plot - Density vs Rural Percentage
- Box Plot for Cleansed and Uncleansed for 2019 and 2021
- Analysis of Massachusetts before and after removal of outliers
- Saved to df_2019.csv, df_2021.csv, df_outliers_2019, and df_outliers_2021.csv

### 501 Analysis of FIPS
- Analysis for the whole United State for 2019 and 2021
  - Average Listing Price
  - Average Listing Price yearly change
- Individual State - Arizona and Massachusetts for 2019 and 2021
  - Average Listing Price
  - Average Listing Price yearly change
  
### 502 Choropleth FIPS
- Choropleth Maps for the whole United States for 2019 and 2021
  - Average Listing Price - refer to 501 Analysis FIPS.ipynb Section 3.1
- Choropleth Maps 
  - Arizona 2019 and 2021
    - Average Listing Price - refer to 501 Analysis FIPS.ipynb Section 4.1 
  - Massachusetts 2019 and 2021
    - Average Listing Price - refer to 501 Analysis FIPS.ipynb Section 4.2 
  
### 503 K-Means PCA (cleansed).ipynb
- Real Estate dataset with removed outliers
- K-means uses Average Listing Price (2019 and 2021), rural percentage (2010) and Density (2020)
- Silhouette Elbow, Cluster Bar Chart, K-Means clustering, Identify ScatterPlot Bubbles and Cluster's Properties
- K-means for 2019 and 2021
  - FIPS
  - Individual States
    - Arizona 
    - Massachusetts
- Saved to df_FIPS_2019.csv, df_FIPS_2021.csv, df_AZ_2019.csv, df_AZ_2021.csv, df_MA_2019.csv, df_MA_2021.csv

### 504 Choropleth K-Means FIPS PCA (cleansed).ipynb
- Choropleth Maps for the whole United States 2019 and 2021 - refer to 503 K-Means PCA (cleansed).ipynb Section 2.1
- Choropleth Maps 
  - Arizona - refer to 503 K-Means PCA (cleansed).ipynb Section 2.2 
  - Massachusetts - refer to 503 K-Means PCA (cleansed).ipynb Section 2.3

### 505 K-Means FIPS PCA (Uncleansed).ipynb
- Real Estate with outliers
- K-Means uses Average Lisitng Price (2019 and 2021), rural percentage (2010) and density (2020)
- Silhouette Elbow, Cluster Bar Chart, K-Means Clustering, Identify Scatter Plot Bubbles
- K-Means for 2019 and 2021
  - FIPS - whole Unites States
  - Individual State Level
    - Arizona 
    - Massachusetts

### 506 K-Means FIPS.ipynb
- Average Lisitng Price (2019 and 2021) and Density (2020)
- Shows Relationship of Density and Rural percentage
- Shows Statistical Model
- Silhouette Elbow, Cluster Bar Chart, K-Means Clustering, Identify Scatter Plot Bubbles
- K-Means 2019 and 2021
  - FIPS - whole United States
  - Individual States
    - Arizona 
    - Masssachusetts

### 601 Analysis State
- Merge the density and real etate dataset
- Merge Average Listing Prie and Average Listing Price Change for 2019 and 2021 and Density
  - Real Estate cleansed dataset
  - Real Estate uncleansed dataset
- Rural percentage is not used because there is no rural percentage in the state level
- Saved to df_2019_ALP.csv, df_20221_ALP.csv, df_outliers_2019_ALP.csv, df_outliers_2021_ALP.csv

### 602 Chroropleth State
- Choropleth Map for the State (Mean)
  - Average Listing Price - Refer to 601 Analysis State.ipynb Section 2.2
  - Average Listing Price Change (%) - Refer to 601 Analysis State.ipynb Section 2.3

### 603 K-Means State.ipynb
- Merge the density and real estate dataset
- Merge Average Listing Price 2019 and 2021 and Density
  - Real estate dataset cleansed
  - Real estate dataset uncleansed
- Silhouette Elbow, Cluster Bar Chart, K-Means Clustering, Identify Scatter Plot Bubbles
- Saved to df_state_2019.csv, df_state_2021.csv, df_outliers_state_2019.csv, df_outliers_state_2021.csv


### 604 Choropleth K-Means State (Cleansed and Uncleansed).ipynb
- Choropleth Map for the State (Mean)
  - Cleansed - refer to 603 K-Means State.ipynb Section 3.1
  - Uncleansed - refer to 603 K-Means State.ipynb Section 5.1 
