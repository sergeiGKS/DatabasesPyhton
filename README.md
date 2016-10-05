#DatabasesPyhton

##Final Project for Using Databases with Python Online Course on Coursera: Using the Google Geocoding API with a Database and Visualizing data on Google Map

#Used softwares and Languages:
Python, SQLite, JavaScript, HTML, Google Map API.


In this project, we are using the Google geocoding API to clean up some user-entered geographic locations of university names and then placing the data(My University, AIMS Senegal) on a Google Map.

We need to install the SQLite browser to view and modify the databases from:
http://sqlitebrowser.org/

##Writing data on database

In the first step we take our input data in the file (where.data) and read it one line at a time, and retreive the geocoded response and store it in a database (geodata.sqlite).

Run the geoload.py program.  
This program will read the input lines in where.data and for each line check to see if it is already in the database and if we don't have the data for the location, call the geocoding API to retrieve the data and store it in the database.

##Visualization 

Once we have some data loaded into geodata.sqlite, we visualize the data using the (geodump.py) program.  This program reads the database and writes tile file (where.js) with the location, latitude, and longitude in the form of executable JavaScript code. 

Open where.html to view the data in a browser

The file (where.html) consists of HTML and JavaScript to visualize a Google Map.  It reads the most recent data in where.js to get the data to be visualized.

