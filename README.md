Weather Data Analysis 

Project Overview
The project analyses rainfall data to explore whether it rains more in Seattle than in another chosen U.S. city - Michigan. In more technical terms, we determine if Seattle receives more precipitation than Michigan.  Using data from from Seattle and Michigan, the analysis compares rainfall patterns over the period January 1, 2018 - December 31, 2022.

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
  - Michigan: https://www.ncei.noaa.gov/cdo-web/datasets/GHCND/stations/GHCND:US1MIMR0016/detail
Description: The above datasets contain daily precipitation measurements recorded between January 1, 2018, and December 31, 2022. Each file includes the following important features we care about as well as other features. The total records for Seattle is about 1600+ and for Michigan ios about 1700+.
The important features or attributes we care about include:
  - DATE - calendar date of observation
  - PRCP - daily precipitation
  - STATION - Weather station ID
  - Name - City/Station name(all data come from one particular station) 
License: (if applicable)
Analysis
Describe the notebooks and/or scripts used to perform the analysis. Specify the order in which the code should be run to reproduce the results.

Results
Include a short discussion of the findings and what they imply.

Authors
Your Name - @Edwin Okwor
github: kembaoak
License
This project is licensed under the MIT License - see the LICENSE file for details.

Acknowledgements
Tools/libraries used: Python, Jupyter Notebook, Pandas , NumPy, Matplotlib, Scikit-learn
Tutorials or papers referenced
Inspiration or collaborators: N/A


