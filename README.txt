Author: Aditya Yaji
********************************************************************************************************************************************
Project Overview: 

Developed a web-application where:
•	The app-user shall be able to specify the search conditions using two fields to represent the pair (business-category, street-name).
•	The search results for top rated Yelp-reviewed places based on the specified filter by the app-user shall be displayed on a webpage.
•	The app-user shall be provided with the capability to view the real-time status for the near-by Divvy docking stations of the selected place 	along with Google map for the current location, the selected place location, and the nearest 3 Divvy docking stations of the selected place.

*********************************************************************************************************************************************
The ChicagoSocialHub folder has 4 folders -
1. backend
    - The backend folder consists of the server.js file (file name in the server).
	
2. backend-build-divvy-status
	- The backend-build-divvy-status folder consists of the python script(divvy_stations_status.ipynb) that is used to connect and store Divvy station status onto the PostgreSQL database.
	
3. backend-build-yelp-reviews
	- The backend-build-yelp-reviews folder consists of the python script(ChicagpSocialHub-Yelp.ipynb) that is used to store Yelp reviews for Chicago Businesses on ElasticSearch database.

4. frontend
	- The frontend folder consists of all code files (.ts, .html, .css) for building the application frontend. 

**************************************
Technologies Used to run application
**************************************
ChicagoSocialHub is a web-based real-time app that uses the following technologies:
1. Angular
2. Node.js/Express
3. PostgreSQL – to store Divvy station status
4. ElasticSearch – to store Yelp reviews for Chicago Businesses

*********************************************
Packages to be installed to run application
*********************************************
1. npm install --save d3
2. npm install -save-dev @types/d3
3. npm install @angular/http –save
4. npm install heatmap.js
5. npm install google-maps

*************************
How to run application
*************************
1. Create your Yelp API Key and update the ipynb script with that key.
2. Create your Google Map API Key and add your Key to the client/Angular frontend file, app.module.ts and index.html
3. Run ChicagoSocialHub-Yelp-reviews.ipynb to create an index to Chicago Business on ElasticSearch database.
4. Run divvy_real-time_status.ipynb to store Divvy Stations data on PostgreSQL database.
5. Run divvy_trips.ipynb file.
6. Execute the following commands from the command line window/terminal:
	- Start ElasticSearch: server from the command prompt
	- Start node.js server: node server
	- Start Angular client: ng serve –open
