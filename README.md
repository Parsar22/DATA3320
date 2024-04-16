# Rainfall Patterns Analysis: Seattle vs New York City

## Description
This project analyzes rainfall patterns between Seattle and New York City (NYC) using weather data collected from Seattle Tacoma airport and JFK airport, respectively. The analysis compares average precipitation levels, seasonal trends, and overall rainfall patterns between the two cities.

## Requirements
- Python 3
- Pandas
- NumPy
- Matplotlib
- Seaborn

## Data

data sets [seattle_rain.csv](https://github.com/Parsar22/DATA3320/blob/955adc4a7585e4c2536447de62af4789d12a41e6/seattle_rain.csv) and [ny_rain.csv](https://github.com/Parsar22/DATA3320/blob/955adc4a7585e4c2536447de62af4789d12a41e6/ny_rain.csv) were downloaded from the National Centers for Environmental Information NOAA Climate Data Online search tool. these data sets were cleaned and used for analysis.
## Data Processing   

The data was cleaned using [this](https://github.com/Parsar22/DATA3320/blob/955adc4a7585e4c2536447de62af4789d12a41e6/Data_preperation.ipynb) colab notebook. 
the steps taken to clean the data are noted below

Loaded weather data for Seattle and New York from CSV files available online into pandas DataFrames.

Examined the structure of the data by looking at the first few rows and using the describe() function to get summary statistics for each column.

Converted the 'DATE' column from string to datetime format using the pd.to_datetime() function.

Removed unnecessary columns such as 'ELEVATION', 'SNOW', 'DAPR', 'MDPR', 'SNWD', 'DASF', and 'MDSF'.

Selected only relevant stations for analysis (Seattle Tacoma Airport and JFK International Airport).

Removed duplicate rows from the data.

Data Joining: Merged the data for Seattle and New York based on the common 'DATE' column using a left join.

Reshaped the data into a tidy format using the pd.melt() function.

Renamed the precipitation columns to reflect the respective cities.

Filled in missing precipitation data for Seattle using the mean precipitation for each day of the year from previous years.

extracted the [clean_seattle_nyc_weather.csv](https://github.com/Parsar22/DATA3320/blob/955adc4a7585e4c2536447de62af4789d12a41e6/clean_seattle_nyc_weather.csv)

## Author 

Parsa Rahimiderimi 
linkedin : https://www.linkedin.com/in/parsa-rahimiderimi

## License 

You are free to use, modify, and distribute the code. If you use this project or its code in your own work, please provide appropriate attribution by citing this repository.
