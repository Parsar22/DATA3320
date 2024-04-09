# DATA3320 Weather Project 

Description : 
The Idea is to compare the amount of rain in Seattle vs NYC and to find out in which city it rains more.


data : 
Seattle_rain.csv and ny_rain.csv are the data we are using for this project
data sets were downloaded from the National Centers for Environmental Information NOAA Climate Data Online search tool. link to the website is provided below :
https://www.ncei.noaa.gov/cdo-web/search?datasetid=GHCND


Data cleaning : 
Data Loading: Loaded weather data for Seattle and New York from CSV files available online into pandas DataFrames.

Data Inspection: Examined the structure of the data by looking at the first few rows and using the describe() function to get summary statistics for each column.

Data Type Conversion: Converted the 'DATE' column from string to datetime format using the pd.to_datetime() function.

Data Cleaning:

Removed unnecessary columns such as 'ELEVATION', 'SNOW', 'DAPR', 'MDPR', 'SNWD', 'DASF', and 'MDSF'.
Selected only relevant stations for analysis (Seattle Tacoma Airport and JFK International Airport).
Removed duplicate rows from the data.
Data Joining: Merged the data for Seattle and New York based on the common 'DATE' column using a left join.

Data Tidying:

Reshaped the data into a tidy format using the pd.melt() function.
Renamed the precipitation columns to reflect the respective cities.

Data Imputation: Filled in missing precipitation data for Seattle using the mean precipitation for each day of the year from previous years.
