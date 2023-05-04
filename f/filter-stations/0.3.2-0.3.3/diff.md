# Comparing `tmp/filter_stations-0.3.2.tar.gz` & `tmp/filter_stations-0.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "filter_stations-0.3.2.tar", last modified: Wed May  3 06:56:42 2023, max compression
+gzip compressed data, was "filter_stations-0.3.3.tar", last modified: Thu May  4 10:47:32 2023, max compression
```

## Comparing `filter_stations-0.3.2.tar` & `filter_stations-0.3.3.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-05-03 06:56:42.947232 filter_stations-0.3.2/
--rw-rw-rw-   0        0        0    39900 2023-05-03 06:56:42.946220 filter_stations-0.3.2/PKG-INFO
--rw-rw-rw-   0        0        0    39594 2023-05-01 20:35:50.000000 filter_stations-0.3.2/README.md
-drwxrwxrwx   0        0        0        0 2023-05-03 06:56:42.907290 filter_stations-0.3.2/filter_stations/
--rw-rw-rw-   0        0        0    36141 2023-05-03 06:56:15.000000 filter_stations-0.3.2/filter_stations/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-03 06:56:42.944069 filter_stations-0.3.2/filter_stations.egg-info/
--rw-rw-rw-   0        0        0    39900 2023-05-03 06:56:42.000000 filter_stations-0.3.2/filter_stations.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      282 2023-05-03 06:56:42.000000 filter_stations-0.3.2/filter_stations.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-03 06:56:42.000000 filter_stations-0.3.2/filter_stations.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       67 2023-05-03 06:56:42.000000 filter_stations-0.3.2/filter_stations.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       92 2023-05-03 06:56:42.000000 filter_stations-0.3.2/filter_stations.egg-info/requires.txt
--rw-rw-rw-   0        0        0       16 2023-05-03 06:56:42.000000 filter_stations-0.3.2/filter_stations.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-03 06:56:42.948217 filter_stations-0.3.2/setup.cfg
--rw-rw-rw-   0        0        0      933 2023-05-03 06:53:56.000000 filter_stations-0.3.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-04 10:47:32.887698 filter_stations-0.3.3/
+-rw-rw-rw-   0        0        0      361 2023-05-04 10:47:32.887202 filter_stations-0.3.3/PKG-INFO
+-rw-rw-rw-   0        0        0       55 2023-05-04 10:44:45.000000 filter_stations-0.3.3/README.md
+drwxrwxrwx   0        0        0        0 2023-05-04 10:47:32.856774 filter_stations-0.3.3/filter_stations/
+-rw-rw-rw-   0        0        0    36858 2023-05-04 10:42:33.000000 filter_stations-0.3.3/filter_stations/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-04 10:47:32.885290 filter_stations-0.3.3/filter_stations.egg-info/
+-rw-rw-rw-   0        0        0      361 2023-05-04 10:47:32.000000 filter_stations-0.3.3/filter_stations.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      282 2023-05-04 10:47:32.000000 filter_stations-0.3.3/filter_stations.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-04 10:47:32.000000 filter_stations-0.3.3/filter_stations.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       67 2023-05-04 10:47:32.000000 filter_stations-0.3.3/filter_stations.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       92 2023-05-04 10:47:32.000000 filter_stations-0.3.3/filter_stations.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       16 2023-05-04 10:47:32.000000 filter_stations-0.3.3/filter_stations.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-04 10:47:32.888298 filter_stations-0.3.3/setup.cfg
+-rw-rw-rw-   0        0        0      933 2023-05-04 10:43:04.000000 filter_stations-0.3.3/setup.py
```

### Comparing `filter_stations-0.3.2/filter_stations/__init__.py` & `filter_stations-0.3.3/filter_stations/__init__.py`

 * *Files 11% similar despite different names*

```diff
@@ -64,21 +64,23 @@
         else:
             return self.__handleApiError(apiRequest)
     
     def get_stations_info(self, station=None, multipleStations=[], countrycode=None):
         """
         Retrieves information about weather stations from an API endpoint and returns relevant information based on the parameters passed to it.
 
-        Args:
-            station (str, optional): Code for a single station to retrieve information for. Defaults to None.
-            multipleStations (list, optional): List of station codes to retrieve information for multiple stations. Defaults to [].
-            countrycode (str, optional): Country code to retrieve information for all stations located in the country. Defaults to None.
+        Parameters:
+        -----------
+        - station (str, optional): Code for a single station to retrieve information for. Defaults to None.
+        - multipleStations (list, optional): List of station codes to retrieve information for multiple stations. Defaults to [].
+        - countrycode (str, optional): Country code to retrieve information for all stations located in the country. Defaults to None.
 
         Returns:
-            pandas.DataFrame: DataFrame containing information about the requested weather stations.
+        -----------
+        - pandas.DataFrame: DataFrame containing information about the requested weather stations.
 
         """
         # Make API request and convert response to DataFrame
         response = self.__request(endpoints['STATION_INFO'], {'sort':'code'})
         info = pd.json_normalize(response['data']).drop('id', axis=1)
         
         # Filter DataFrame based on parameters
@@ -94,15 +96,16 @@
 
         
     def get_variables(self):
         """
         Retrieves information about available weather variables from an API endpoint.
 
         Returns:
-            dict: Dictionary containing information about available weather variables, keyed by variable shortcode.
+        -----------
+        - dict: Dictionary containing information about available weather variables, keyed by variable shortcode.
         """
         # Make API request and create dictionary of variables
         response = self.__request(endpoints['VARIABLES'], {})
         variables = {}
         if 'data' in response and isinstance(response['data'], list):
             for element in response['data']:
                 variables[element['variable']['shortcode']] = element['variable']
@@ -132,20 +135,22 @@
     def raw_measurements(self, station, startDate=None, endDate=None, variables=None):
         return self.get_measurements(station, startDate=startDate, endDate=endDate, variables=variables, dataset='raw')
     
     def k_neighbours(self, station, number=5):
         """
         Returns a dictionary of the nearest neighbouring stations to the specified station.
 
-        Args:
-            station (str): Code for the station to find neighbouring stations for.
-            number (int, optional): Number of neighbouring stations to return. Defaults to 5.
+        Parameters:
+        -----------
+        - station (str): Code for the station to find neighbouring stations for.
+        - number (int, optional): Number of neighbouring stations to return. Defaults to 5.
 
         Returns:
-            dict: Dictionary containing the station codes and distances of the nearest neighbouring stations.
+        -----------
+        - dict: Dictionary containing the station codes and distances of the nearest neighbouring stations.
         """
         # Get latitude and longitude of specified station
         lon, lat = self.get_stations_info(station)[['location.longitude', 'location.latitude']].values[0]
         
         # Calculate distances to all other stations and sort by distance
         infostations = self.get_stations_info()
         infostations['distance'] = infostations.apply(lambda row: hs.haversine((lat, lon), (row['location.latitude'], row['location.longitude'])), axis=1)
@@ -155,38 +160,42 @@
         return dict(infostations[['code', 'distance']].head(number).values[1:])
     
     # trained models in stored in mongoDB
     def trained_models(self, columns=None):
         """
         Retrieves trained models from the MongoDB.
 
-        Args:
-            columns (list of str, optional): List of column names to include in the returned DataFrame. 
+        Parameters:
+        -----------
+        - columns (list of str, optional): List of column names to include in the returned DataFrame. 
                 If None, all columns are included. Defaults to None.
 
         Returns:
-            pandas.DataFrame: DataFrame containing trained models with the specified columns.
+        -----------
+        - pandas.DataFrame: DataFrame containing trained models with the specified columns.
         """
         reqUrl = "https://tahmorqctest.eu-de.mybluemix.net/api/models" # endpoint
         response = self.__request(reqUrl, {})
         if columns:
             return pd.DataFrame(response.json())[columns]
         else:
             return pd.DataFrame(response.json())
 
     
     def aggregate_variables(self, dataframe):
         """
         Aggregates a pandas DataFrame of weather variables by summing values across each day.
 
-        Args:
-            dataframe (pandas.DataFrame): DataFrame containing weather variable data.
+        Parameters:
+        -----------
+        - dataframe (pandas.DataFrame): DataFrame containing weather variable data.
 
         Returns:
-            pandas.DataFrame: DataFrame containing aggregated weather variable data, summed by day.
+        -----------
+        - pandas.DataFrame: DataFrame containing aggregated weather variable data, summed by day.
         """
         # Reset index and rename columns
         dataframe = dataframe.reset_index()
         dataframe.rename(columns={'index':'Date'}, inplace=True)
         
         # Group by date and sum values
         return dataframe.groupby(pd.Grouper(key='Date', axis=0, freq='1D')).sum()
@@ -195,30 +204,30 @@
     # Get the variables only
     def get_measurements(self, station, startDate=None, endDate=None, variables=None, dataset='controlled', aggregate=False):
             """
             Get measurements from a station.
 
             Parameters:
             -----------
-            station: str
+            - station: str
                 The station ID.
-            startDate: str, optional
+            - startDate: str, optional
                 The start date of the measurement period in the format 'YYYY-MM-DD'.
-            endDate: str, optional
+            - endDate: str, optional
                 The end date of the measurement period in the format 'YYYY-MM-DD'.
-            variables: list, optional
+            - variables: list, optional
                 The variables to retrieve measurements for. If None, all variables are retrieved.
-            dataset: str, optional
+            - dataset: str, optional
                 The dataset to retrieve measurements from. Default is 'controlled'.
-            aggregate: bool, optional
+            - aggregate: bool, optional
                 Whether to aggregate the measurements by variable. Default is False.
 
             Returns:
             --------
-            pd.DataFrame
+            - pd.DataFrame
                 A DataFrame containing the measurements.
             """            
             #print('Get measurements', station, startDate, endDate, variables)
             endpoint = 'services/measurements/v2/stations/%s/measurements/%s' % (station, dataset)
 
             dateSplit = self.__splitDateRange(startDate, endDate)
             series = []
@@ -336,25 +345,28 @@
     
     # retrieve data from multiple at a time
     def multiple_measurements(self, stations_list, csv_file, startDate, endDate, variables, dataset='controlled'):
         """
         Retrieves measurements for multiple stations and saves the aggregated data to a CSV file.
 
         Parameters:
-            stations_list (list): A list of strings containing the names of the stations to retrieve data from.
-            csv_file (str): The name of the CSV file to save the data to.
-            startDate (str): The start date for the measurements, in the format 'yyyy-mm-dd'.
-            endDate (str): The end date for the measurements, in the format 'yyyy-mm-dd'.
-            variables (list): A list of strings containing the names of the variables to retrieve.
-            dataset (str): The name of the dataset to retrieve the data from. Default is 'controlled'.
+        -----------
+        - stations_list (list): A list of strings containing the names of the stations to retrieve data from.
+        - csv_file (str): The name of the CSV file to save the data to.
+        - startDate (str): The start date for the measurements, in the format 'yyyy-mm-dd'.
+        - endDate (str): The end date for the measurements, in the format 'yyyy-mm-dd'.
+        - variables (list): A list of strings containing the names of the variables to retrieve.
+        - dataset (str): The name of the dataset to retrieve the data from. Default is 'controlled'.
 
         Returns:
-            df (pandas.DataFrame): A DataFrame containing the aggregated data for all stations.
+        -----------
+        - df (pandas.DataFrame): A DataFrame containing the aggregated data for all stations.
 
         Raises:
+
             ValueError: If stations_list is not a list.
         """
         error_dict = dict()
         if isinstance(stations_list, list):
             df_stats = []
             
             for station in stations_list:
@@ -392,41 +404,43 @@
     # Get the centre point of the address
     def centre_point(self, address):
         """
         This method retrieves the latitude and longitude coordinates of a given address using the Nominatim API.
         
         Parameters:
         -----------
-        address : str
+        - address : str
             The address of the location you want to retrieve the coordinates for.
             
         Returns:
         --------
-        Tuple (float, float)
+        - Tuple (float, float)
             The latitude and longitude coordinates of the location.
         """
         url = 'https://nominatim.openstreetmap.org/search/' + urllib.parse.quote(address) +'?format=json'
         return requests.get(url).json()[0]['lat'], requests.get(url).json()[0]['lon']
 
     # Get the new radius of the address
     def calculate_new_point(self, lat, lon, distance, bearing):
         """
         Calculates a new geographic point based on the given latitude, longitude,
         distance and bearing.
 
         Parameters:
-            lat (float): The latitude of the starting point in decimal degrees.
-            lon (float): The longitude of the starting point in decimal degrees.
-            distance (float): The distance in kilometers from the starting point to the new point.
-            bearing (float): The bearing in degrees from the starting point to the new point,
-                measured clockwise from true north.
+        -----------
+        - lat (float): The latitude of the starting point in decimal degrees.
+        - lon (float): The longitude of the starting point in decimal degrees.
+        - distance (float): The distance in kilometers from the starting point to the new point.
+        - bearing (float): The bearing in degrees from the starting point to the new point,
+            measured clockwise from true north.
 
         Returns:
-            Tuple[float, float]: A tuple containing the latitude and longitude of the new point,
-            respectively, in decimal degrees.
+        -----------
+        - Tuple[float, float]: A tuple containing the latitude and longitude of the new point,
+        respectively, in decimal degrees.
         """
         distance = distance * 1000
         # Convert degrees to radians
         lat = math.radians(lat)
         lon = math.radians(lon)
         bearing = math.radians(bearing)
         
@@ -450,20 +464,22 @@
 
     # Get the bounding box of the address
     def compute_filter(self, lat, lon, distance):
         """
         Calculates the bounding box coordinates for a given location and distance.
 
         Parameters:
-        lat (float): The latitude of the location.
-        lon (float): The longitude of the location.
-        distance (float): The distance from the location, in kilometers, to the edge of the bounding box.
+        -----------
+        - lat (float): The latitude of the location.
+        - lon (float): The longitude of the location.
+        - distance (float): The distance from the location, in kilometers, to the edge of the bounding box.
 
         Returns:
-        A tuple containing four floats representing the bounding box coordinates: (min_lat, min_lon, max_lat, max_lon).
+        -----------
+        - A tuple containing four floats representing the bounding box coordinates: (min_lat, min_lon, max_lat, max_lon).
         """
         points = []
         g1 = []
         for i in range(0, 360, 45):
             points.append(self.calculate_new_point(lat, lon, distance, i))
         g1 = [min(p[0] for p in points), min(p[1] for p in points)]
         g2 = [max(p[0] for p in points), max(p[1] for p in points)]
@@ -474,22 +490,24 @@
 
 
     def filter_stations(self, address, distance, startDate=None, endDate=None, csvfile='KEcheck3.csv'):
         """
         This method filters weather station data within a certain distance from a given address.
         
         Parameters:
-        address (str): Address to center the bounding box around.
-        distance (float): The distance (in kilometers) from the center to the edge of the bounding box.
-        startDate (str): The start date for filtering the weather station data in the format 'YYYY-MM-DD'.
-        endDate (str): The end date for filtering the weather station data in the format 'YYYY-MM-DD'.
-        csvfile (str): The name of the csv file containing the weather station data.
+        -----------
+        - address (str): Address to center the bounding box around.
+        - distance (float): The distance (in kilometers) from the center to the edge of the bounding box.
+        - startDate (str): The start date for filtering the weather station data in the format 'YYYY-MM-DD'.
+        - endDate (str): The end date for filtering the weather station data in the format 'YYYY-MM-DD'.
+        - csvfile (str): The name of the csv file containing the weather station data.
         
         Returns:
-        pandas.DataFrame: The filtered weather station data within the bounding box.
+        -----------
+        - pandas.DataFrame: The filtered weather station data within the bounding box.
         """     
         lat, lon = self.centre_point(address)
         min_lat, min_lon, max_lat, max_lon = self.compute_filter(float(lat), float(lon), distance)
         stations = super().get_stations_info()
         bounds = list(stations['code'][(stations['location.longitude'] >= min_lon)
                                         & (stations['location.longitude'] <= max_lon)
                                         & (stations['location.latitude'] >= min_lat)
@@ -516,20 +534,22 @@
 
 
     # A list of filtered stations
     def filter_stations_list(self, address, distance=100):
         """
         Filters stations based on their proximity to a given address and returns a list of station codes that fall within the specified distance.
         
-        Args:
-            address (str): Address to filter stations by.
-            distance (float, optional): Maximum distance (in kilometers) between the stations and the address. Default is 100 km.
+        Parameters:
+        -----------
+        - address (str): Address to filter stations by.
+        - distance (float, optional): Maximum distance (in kilometers) between the stations and the address. Default is 100 km.
         
         Returns:
-            List of station codes that fall within the specified distance from the given address.
+        -----------
+        - List of station codes that fall within the specified distance from the given address.
         """
         return list(set([i.split('_')[0] for i in self.filter_stations(f'{address}', distance).columns if i.split('_')[-1] != 'clogFlag']))
 
     
 
 # A different class for visualisations
 class Interactive_maps(retreive_data):
@@ -537,19 +557,21 @@
     def __init__(self, apiKey, apiSecret):
         super().__init__(apiKey, apiSecret)
 
     def draw_map(self, map_center):
         """
         Creates a Folium map centered on the specified location and adds markers for each weather station in the area.
 
-        Args:
-            map_center: a tuple with the latitude and longitude of the center of the map
+        Parameters:
+        -----------
+        - map_center: a tuple with the latitude and longitude of the center of the map
 
         Returns:
-            A Folium map object
+        -----------
+        - A Folium map object
         """
 
         #  retrieve the stations data
         stations = super().get_stations_info()[['code', 'location.longitude', 'location.latitude']]
         # create a map centered on a specific location
 
         my_map = folium.Map(location=map_center, min_zoom=5, max_zoom=30, zoom_start=12, tiles='cartodbpositron')
@@ -566,22 +588,24 @@
 
 
     def animation_image(self, sensors,  start_date, end_date, day=100, T=10, interval=500, data=None):
         '''
         Creates an animation of pollutant levels for a given range of days and valid sensors.
 
         Parameters:
-        data (DataFrame): A pandas DataFrame containing pollution data.
-        sensors (list): A list of valid sensor names.
-        day (int): The starting day of the animation (default is 100).
-        T (int): The range of days for the animation (default is 10).
-        interval (int): The interval between frames in milliseconds (default is 500).
+        -----------
+        - data (DataFrame): A pandas DataFrame containing station data defaults to none reads KEcheck3 if none.
+        - sensors (list): A list of valid sensor names.
+        - day (int): The starting day of the animation (default is 100).
+        - T (int): The range of days for the animation (default is 10).
+        - interval (int): The interval between frames in milliseconds (default is 500).
 
         Returns:
-        HTML: An HTML object containing the animation.
+        -----------
+        - HTML: An HTML object containing the animation.
         '''
         if not data:
             data = pd.read_csv('KEcheck3.csv')
             data['Date'] = pd.to_datetime(data['Date'])
             data = data.loc[(data['Date'] >= start_date) & (data['Date'] <= end_date)]
 
         
@@ -613,23 +637,25 @@
     
     # create animation grid
     def animation_grid(self, mu_pred, xi, xj, valid_station_df, clogged_station_df, T=10):
         """
         Creates an animation of the predicted data on a grid over time.
 
         Parameters:
-        mu_pred (ndarray): The predicted data on a grid over time.
-        xi (ndarray): The x-coordinates of the grid.
-        xj (ndarray): The y-coordinates of the grid.
-        valid_station_df (DataFrame): A DataFrame containing the information of the valid stations.
-        clogged_station_df (DataFrame): A DataFrame containing the information of the clogged stations.
-        T (int): The number of time steps.
+        -----------
+        - mu_pred (ndarray): The predicted data on a grid over time.
+        - xi (ndarray): The x-coordinates of the grid.
+        - xj (ndarray): The y-coordinates of the grid.
+        - valid_station_df (DataFrame): A DataFrame containing the information of the valid stations.
+        - clogged_station_df (DataFrame): A DataFrame containing the information of the clogged stations.
+        - T (int): The number of time steps.
 
         Returns:
-        HTML: The animation as an HTML object.
+        -----------
+        - HTML: The animation as an HTML object.
         """
         fig, ax = plt.subplots()
 
         def animate(t):
             ax.clear()
             ax.set_title('Time step {}'.format(t))
             ax.pcolor(xi, xj, mu_pred[:, t:t+1].reshape(xi.shape), shading='auto')
@@ -643,19 +669,21 @@
 
 
 
     def plot_station(self, ws, df_rainfall):
         """
         Plot the rainfall data for a specific weather station.
 
-        Args:
+        Parameters:
+        -----------
         - ws: string, the code of the weather station to plot
         - df_rainfall: DataFrame, a pandas DataFrame with rainfall data
 
         Returns:
+        -----------
         - None if no data is available for the specified station
         - a Matplotlib figure showing rainfall data for the specified station otherwise
         """
         # filter columns based on station code and type (sensor or clog flag)
         sensors = [x for x in list(df_rainfall.keys()) if ws in x and 'clog' not in x]
         clog_flags = [x for x in list(df_rainfall.keys()) if ws in x and 'clog' in x]
 
@@ -687,19 +715,21 @@
 
 
     # Encode the image
     def encode_image(self, ws, df_rainfall):
         """
         Encodes a station's rainfall data plot as a base64-encoded image.
 
-        Args:
+        Parameters:
+        -----------
         - ws (str): the code for the station to encode the image for
         - df_rainfall (pandas.DataFrame): a DataFrame containing the rainfall data for all stations
         
         Returns:
+        -----------
         - str: a string containing an HTML image tag with the encoded image data, or a message indicating no data is available for the given station
         """
         figure = self.plot_station(ws, df_rainfall)
         if figure is not None:
             figure.tight_layout()
             buf = BytesIO()
             figure.savefig(buf, format='png')
@@ -715,38 +745,38 @@
 
     def get_map(self, subset_list, start_date=None, end_date=None, data_values=False, csv_file='KEcheck3.csv', min_zoom=8, max_zoom=11, width=2000, height=2000, png_resolution=300):
         """
         Creates a Folium map showing the locations of the weather stations in the given subsets.
 
         Parameters:
         -----------
-        subset_list : list of lists of str
+        - subset_list : list of lists of str
             List of subsets of weather stations, where each subset is a list of station codes.
-        start_date : str, optional
+        - start_date : str, optional
             Start date in the format YYYY-MM-DD, default is None.
-        end_date : str, optional
+        - end_date : str, optional
             End date in the format YYYY-MM-DD, default is None.
-        data_values : bool, optional
+        - data_values : bool, optional
             If True, the map markers will display a plot of rainfall data, default is False.
-        csv_file : str, optional
+        - csv_file : str, optional
             The name of the CSV file containing the rainfall data, default is 'KEcheck3.csv'.
-        min_zoom : int, optional
+        - min_zoom : int, optional
             The minimum zoom level of the map, default is 8.
-        max_zoom : int, optional
+        - max_zoom : int, optional
             The maximum zoom level of the map, default is 11.
-        width : int, optional
+        - width : int, optional
             The width of the map in pixels, default is 850.
-        height : int, optional
+        - height : int, optional
             The height of the map in pixels, default is 850.
-        png_resolution : int, optional
+        - png_resolution : int, optional
             The resolution of the PNG image if data_values is True, default is 300.
 
         Returns:
         --------
-        my_map : folium.folium.Map
+        - my_map : folium.folium.Map
             A Folium map object showing the locations of the weather stations in the given subsets.
         """
         # Read the csv file 
         df_rainfall = pd.read_csv(csv_file)
         df_rainfall['Date'] = pd.to_datetime(df_rainfall['Date'])
         df_rainfall= df_rainfall.set_index('Date')
         if start_date and end_date:
```

### Comparing `filter_stations-0.3.2/setup.py` & `filter_stations-0.3.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(
     name='filter_stations',
-    version='0.3.2',
+    version='0.3.3',
     packages=find_packages(),
     include_package_data=True,
     description='Making it easier to navigate and clean station data',
     author='Austin Kaburia',
     author_email='kaburiaaustin1@gmail.com',
     url='https://github.com/kaburia/Packaging/tree/main/filter_stations',
     install_requires=[
```

