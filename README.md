# NASA_Final
**Title: NASA Fire Data Analysis and Visualization**

## Introduction
This Python script analyzes and visualizes NASA's fire incident data using various libraries such as Pandas, Geopandas, and Matplotlib. The code fetches real-time fire incident data from NASA's API, processes the data, calculates damaged areas, and presents the findings through interactive visualizations.

## Code Overview

### Libraries Used
- **Requests:** For making HTTP requests to fetch data from NASA's API.
- **Pandas:** For data manipulation and analysis, particularly using dataframes.
- **NumPy:** For numerical operations.
- **Geopandas:** For handling geographical data and visualizations.
- **Matplotlib:** For creating plots and visualizations.

### Functions and Processes

#### 1. **Data Fetching**
- The script fetches fire incident data from NASA's API using a specific API key.
- The fetched data is displayed as a Pandas dataframe.

#### 2. **Data Preprocessing**
- The script preprocesses the raw data, selecting relevant columns like latitude, longitude, brightness temperature, fire radiative power, and acquisition date.
- The acquisition date is converted to a datetime format for easier manipulation.

#### 3. **Damage Area Calculation**
- The script calculates the damaged area using latitude and longitude data, creating a polygon and computing its area in square kilometers.

#### 4. **Data Visualization**
- The script visualizes fire incidents on a world map, highlighting the locations of incidents.

#### 5. **Time Series Analysis**
- The script analyzes the change in damaged area over time for specific countries (India, Argentina, USA) and plots it against the number of fire incidents.

### Code Execution

#### 1. **Fetching Country Data**
- The script fetches a list of countries and their geometrical data from NASA's API.

#### 2. **Iterative Country Analysis**
- The script iterates through specific countries (India, Argentina, USA).
- For each country, it fetches fire incident data and processes it.
- It calculates the damaged area for each date using latitude and longitude information.
- It plots a graph displaying the change in damaged area over time.

#### 3. **Visualization**
- The script visualizes the fire incidents on a world map using Geopandas and Matplotlib.
- The incidents are represented as red markers on the map.

## Conclusion
This Python script provides a comprehensive analysis and visualization of NASA's real-time fire incident data. It enables users to understand the geographical distribution of fire incidents, analyze their impact over time, and make data-driven decisions regarding fire management and prevention efforts.
