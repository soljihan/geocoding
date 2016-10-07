This project uses the Google Geocoding API with database created in
SQLite to visualize the data on Google Map

'geoload.py' program connects to 'geodata' database
and creates 'Locations' table to insert address and geodata

'where.data' contains the user-input of locations to be visualized

'geoload.py' reads each line in the 'where.data' file
and uses the Google Geocoding API to retrieve the geodata
and converts that into a json file

Address and geodata of each location is inserted into database

'geodump.py' connects to the 'geodata' database
The files reads the json file and writes out 'where.js' file using the information
in the form of executable Javascript file

'where.html' uses the 'where.js' file to create a Google Map
with user-entered locations