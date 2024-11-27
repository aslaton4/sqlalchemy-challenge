# sqlalchemy-challenge

## Overview
### This project asked for students to act as a traveler that is peparing to visit Hawaii. In preparation for the trip it required me to analyze climate data for Hawaii and build a Flask API for the results. The dataset provided included historical weather data, such as temperature and precipitation, that was gathered from various weather stations across Hawaii.

### This project was broken into 2 separate sections as follows: 
- Climate data analysis - completed by performing exploration and analysis using python, pandas, sqlalchemy, and Matplotlib.
- Development of a Flask API - this allowed for providing the results through accessible web routes. 

## Part 1 
### Climate Data analysis
- SQLite databse was connected using SQLAlchemy.
- The database schema was shown to map both measurement and station tables.
- The most recent 12 months of precipitation data was queried and loaded into a Pandas Dataframe, sorted by date. 
- A time-series graph of preciptitaion results were plotted. 
- A summary of the statistics for the preciptiation data was calculated. 
- The number of weather stations in total were calculated and identified the most active station by the number of observations. 
- Temperatures for the most active station was queried for the past 12 month time frame and visualized using a histogram. 

## Part 2
### Flask API routes
- / (Homepage)
    - Displays a list of all available API routes.
- /api/v1.0/precipitation   
    - Shows the last 12 months of precipitation information as a JSON dictionary with the dates used as keys and precipitation values as values.
- /api/v1.0/stations
    - Returns a JSON list of all weather stations in the provided dataset. 
- /api/v1.0/tobs
    - Returns a JSON list of temperature observations for the most active station over the past 12 months. 
- /api/v1.0/<start>
    - Takes a start date (YYYY-MM-DD) and returns a JSON object with the minimum, average, and maximum temperatures for all of the dates that are >= the start date.
- /api/v1.0/<start>/<end>
    - Takes a start date and an end date (YYYY-MM-DD) and returns a JSON object with the minimum, average, and maximum temps for dates between the start and ends dates. 

## Resources
- Class lecture and watching of recordings
- Youtube
- Assigned group 
- Chatgpt