# sqlalchemy-challenge
The "SurfsUp" directory comprises the Jupyter Notebook "climate.ipynb," the Python script "app.py," and a "Resources" folder containing the "hawaii.sqlite" database, "hawaii_measurements.csv," and "hawaii_stations.csv" files.

**Analyze and Explore Climate Data**
Exploration and analysis of climate data were conducted on the "hawaii.sqlite" database. The Jupyter Notebook "climate.ipynb" was specifically crafted for precipitation and station analysis. Additionally, the Python script "app.py" was developed to build a climate app, featuring a Flask API with five routes that provide JSON lists containing pertinent climate information.

*Precipiation Analysis*
-Pandas DataFrame created using ORM queried Data from past 12 months

-Plotted results below: 
<img width="624" alt="Screenshot 2023-12-12 at 5 39 30 PM" src="https://github.com/stelladrose49/sqlalchemy-challenge/assets/141170388/af835a20-0701-4c40-8f97-0be9316b8368">

-A summary statistics table was printed for the precipitation data for the previous 12 months below:
<img width="164" alt="Screenshot 2023-12-12 at 5 37 08 PM" src="https://github.com/stelladrose49/sqlalchemy-challenge/assets/141170388/c9acdeba-2883-4df5-9559-1735ea8066a6">

*Station Analysis*
-All active stations and numbered counts are listed below in descending order:
[('USC00519281', 2772),
 ('USC00519397', 2724),
 ('USC00513117', 2709),
 ('USC00519523', 2669),
 ('USC00516128', 2612),
 ('USC00514830', 2202),
 ('USC00511918', 1979),
 ('USC00517948', 1372),
 ('USC00518838', 511)]

 -Last 12 months of temp. observation for most active station, USC00519281, were queried and plotted on the histogram below:
 <img width="872" alt="Screenshot 2023-12-12 at 5 43 46 PM" src="https://github.com/stelladrose49/sqlalchemy-challenge/assets/141170388/349bc57b-3b29-4b36-8f31-d6caf4fc0779">

*Design Climate API App*

#1. /
-Start at the homepage.
-List all the available routes.

#2. /api/v1.0/precipitation
-Convert the query results from your precipitation analysis (i.e. retrieve only the last 12 months of data) to a dictionary using date as the key and prcp as the value.
-Return the JSON representation of your dictionary.

#3. /api/v1.0/stations
-Return a JSON list of stations from the dataset.

#4. /api/v1.0/tobs
-Query the dates and temperature observations of the most-active station for the previous year of data.
-Return a JSON list of temperature observations for the previous year.

#5. /api/v1.0/<start> and /api/v1.0/<start>/<end>
-Return a JSON list of the minimum temperature, the average temperature, and the maximum temperature for a specified start or start-end range.
-For a specified start, calculate TMIN, TAVG, and TMAX for all the dates greater than or equal to the start date.
-For a specified start date and end date, calculate TMIN, TAVG, and TMAX for the dates from the start date to the end date, inclusive.
