# sqlalchemy-challenge
The "SurfsUp" directory comprises the Jupyter Notebook "climate.ipynb," the Python script "app.py," and a "Resources" folder containing the "hawaii.sqlite" database, "hawaii_measurements.csv," and "hawaii_stations.csv" files.

**Analyze and Explore Climate Data**
Exploration and analysis of climate data were conducted on the "hawaii.sqlite" database. The Jupyter Notebook "climate.ipynb" was specifically crafted for precipitation and station analysis. Additionally, the Python script "app.py" was developed to build a climate app, featuring a Flask API with five routes that provide JSON lists containing pertinent climate information.

*Precipiation Analysis*
-Pandas DataFrame created using ORM queried Data from past 12 months
<div>
<style scoped>
    .dataframe tbody tr th:only-of-type {
        vertical-align: middle;
    }

    .dataframe tbody tr th {
        vertical-align: top;
    }

    .dataframe thead th {
        text-align: right;
    }
</style>
<table border="1" class="dataframe">
  <thead>
    <tr style="text-align: right;">
      <th></th>
      <th>precipitation</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <th>count</th>
      <td>2021.000000</td>
    </tr>
    <tr>
      <th>mean</th>
      <td>0.177279</td>
    </tr>
    <tr>
      <th>std</th>
      <td>0.461190</td>
    </tr>
    <tr>
      <th>min</th>
      <td>0.000000</td>
    </tr>
    <tr>
      <th>25%</th>
      <td>0.000000</td>
    </tr>
    <tr>
      <th>50%</th>
      <td>0.020000</td>
    </tr>
    <tr>
      <th>75%</th>
      <td>0.130000</td>
    </tr>
    <tr>
      <th>max</th>
      <td>6.700000</td>
    </tr>
  </tbody>
</table>
</div>

