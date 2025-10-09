Does It Rain More in Seattle or Detroit? A Statistical and Visual Exploration of Rainfall Patterns betwen Seattle and Detroit(2018-2022)

Project Overview
The project analyses rainfall data to explore whether it rains more in Seattle than in another chosen U.S. city - Detroit. In more technical terms, we determine if Seattle receives more precipitation than Detroit.  Using data from from Seattle and Detroit, the analysis compares rainfall patterns over the period January 1, 2018 - December 31, 2022. We were able to arrive at a conclusion 

Provide a short and concise overview of the project. Mention the problem it solves, the data used, and the key outcomes or findings.

Objective: Compare precipitation in Seattle with another city to test assumptions about rainfall patterns.
Domain: Environmental Science/Climate Data
Key Techniques: Data cleaning, exploratory data analysis(EDA), time series visualization, and statistical comparison. 

Project Structure
├── data/                 # Raw and processed data
├── code/                 # Jupyter notebooks and Python scripts
├── reports/              # Generated reports and visualizations
├── requirements.txt      # Dependencies
└── README.md             # Project documentation
Data
Source: Link to the data source(s)
  - Seattle: https://www.ncei.noaa.gov/cdo-web/datasets/GHCND/stations/GHCND:US1WAKG0225/detail
  - Detroit: https://www.ncei.noaa.gov/cdo-web/datasets/GHCND/stations/GHCND:US1MIMR0016/detail
Description: The data used in this analysis were obtained from the National Oceanic and Atmospheric Administration (NOAA), a U.S. government agency responsible for collecting and maintaining environmental data. Specifically, daily precipitation data for both cities were sourced from the National Centers for Environmental Information (https://www.ncei.noaa.gov/cdo-web/search). Using the search tool provided on the website, we selected the Daily Summaries dataset, which includes daily precipitation information for each city. The selected period spans from January 1, 2018, to December 31, 2022, providing a sufficient sample to draw conclusions about general rainfall patterns.

The important attributes we care about in our analysis of our dataset include: 
  - DATE - calendar date of observation
  - PRCP - daily precipitation

License: (if applicable)
Analysis
After the data was successfully imported as a data frame, it was cleaned to ensure there were no missing values. Missing values were then replaced with the mean precipitation for that particular date across the five years, as leaving them blank would have resulted in incomplete or invalid analysis. It was also important to ensure that the date and precipitation columns were in the correct formats (date in datetime format and precipitation in inches). The data frames for both cities were merged to allow a more direct comparison of daily precipitation levels. The cleaned data was then exported for further analysis. 
In the exploratory data analysis, we used descriptive statistics, a pie chart, and a bar chart to draw inferences from our data. Descriptive statistics from Figure 1.1 were used to answer questions such as how many days of rainfall data were recorded, which city receives more rain on a daily average, how much daily rainfall varies in each city, and how the average rainfall in Seattle compares to that in Detroit. The pie chart in Figure 1.2 provides a visual comparison of the composition of total precipitation for Detroit and Seattle over the five-year period, helping us better understand the overall distribution of rainfall. A bar chart was also used to visualize the monthly proportion of days with precipitation, which allows us to identify seasonal trends and compare rainfall patterns across months.
All the steps performed during exploratory data analysis are saved in 'Seattle_Detroit_Weather_Data_Project.ipynb' which can be found in code section of this repository. 


Data Preparation
Data was cleansed by ensuring that our datatypes for the attributes of interest were consistent (date as datetime type and precipitation in inches). 
Missing/Nan values were identified and handled accordingly by replacing NaN values with the means for for that particular day over the time period.
The dataframes of both cities were merged using 'DATE' column using outer join to allow a more direct comparison of daily precipitation levels.
The clean data was exported as 'clean_seattle_detroit_weather.csv' (can be found in the data folder)

Note: The notebook 'Seattle_Detroit_Weather_Data_Project.ipynb' saved in the code folder is where our data analysis were done. 


Analysis 
Most of the analysis were done on Jupyter Notebook - 'Seattle_Detroit_Weather_Data_Project.ipynb' which you can find in the code folder in this repository.
In the exploratory data analysis, we used descriptive statistics, a pie chart, and a bar chart to draw inferences from our data. Descriptive statistics from Figure 1.1 were used to answer questions such as how many days of rainfall data were recorded, which city receives more rain on a daily average, how much daily rainfall varies in each city, and how the average rainfall in Seattle compares to that in Detroit. The pie chart in Figure 1.2 provides a visual comparison of the composition of total precipitation for Detroit and Seattle over the five-year period, helping us better understand the overall distribution of rainfall. A bar chart was also used to visualize the monthly proportion of days with precipitation, which allows us to identify seasonal trends and compare rainfall patterns across months.

Results
The data from Figure 1.2 shows that there are an equal number of records for both cities. Seattle has a higher daily mean precipitation than Detroit, with values of 0.113 inches for SEA and 0.085 inches for DTW. The minimum values indicate that both cities experience days without rain, as both have 0.0 inches recorded. About 25% of days in both cities have no rain(1st quartile). Approximately 25% of days in both cities have no rain (1st quartile). However, around 50% of days in Detroit are dry, while in Seattle, 50% of days receive about 0.01 inches of precipitation. The 75th percentile indicates that Detroit receives about 0.04 inches of rainfall on wetter days, compared to 0.12 inches in Seattle. The maximum daily precipitation is the same for both cities, at 2.6 inches.

Figure 1.3 illustrates the monthly proportion of days with precipitation in Seattle and Detroit, with asterisks indicating months where statistical tests revealed significant differences between the two cities. 

Some key observations include: 
The data shows that there are distinct seasonal patterns between the two cities. From December through March, Seattle consistently demonstrates a higher proportion of rain days compared to Detroit. The different climates experienced play a major role, as Seattle’s climate brings more frequent winter rainfall, while Detroit’s continental climate results in more winter precipitation in the form of snow, which is not measured in liquid precipitation records.

The marked months (indicated by asterisks) highlight where the difference in precipitation frequency is statistically significant. During the summer months, Seattle experiences significantly less rainfall than in winter. In Detroit, the proportion of rainy days appears relatively consistent, with values ranging between 0.2 and 0.4.


Authors
Your Name - @Edwin Okwor
github: kembaoak
License
This project is licensed under the MIT License - see the LICENSE file for details.

Acknowledgements
Tools/libraries used: Python, Jupyter Notebook, Pandas , NumPy, Matplotlib, Scikit-learn, VS Code 
Tutorials or papers referenced
Inspiration or collaborators: N/A








