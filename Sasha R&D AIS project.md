# Sasha R&D AIS project

##Projects

These are the way that I classified the work early on in oue conversation. Based on recent conversations and your research feel free to modify the projects.

1. AIS market assessment - Complete by February 27th - $500
 - project description: study market structuree of AIS systems, identify potential partners, customers and opportunities,
 - goals: finalize specification of the product by estimating access modes, potential traffic, priority of the tasks
 - deliverables: pdf with description of user profile, market size, product description, revenue model for each API product. 
 - results: collected data about AIS and s-AIS providers, their web-analytics, navigation mobile apps; contacted to major companies to get more details.
 - https://github.com/akudrya/AIS/blob/master/s-AIS%20market%20research.pdf

2. Prototype imagery and AIS solutions - Complete by March 6th - $2000
 - a. Project description:create a prototype application for matching vessels' coordinates and satellite images
 - b. project description:development of an algorithm for combining satellite images with AIS data
 - goals: check how satellite imagery can be enriched by AIS data
 - deliverables: develope A. proof of concept and B. MVP for finding all satellite images having a given vessel and all the vessels that are located on a satellite image.
 - results: researched articles about detection ships on satellite images, proposed applications of AIS+Landsat data, designed illustrations of how ships can be vizualized on a Landsat image, developed a first mapbox representation of AIS+Landsat data and search, planned how can system work, found and launched data sources.
 - https://github.com/akudrya/AIS/blob/master/Landsat%20Project/Use%20Cases/Landsat%20use%20cases%2003:17.pdf
 - https://github.com/akudrya/AIS/blob/master/Landsat%20Project/Use%20Cases/Landsat%20use%20cases%2003:16.pdf
 - https://github.com/akudrya/AIS/blob/master/Landsat%20Project/LandsatSearchVer1/js/app.js

3. Demo API using static data - $2000
 - project description: development of demo API using static data in web-browser with UI and as API provding data in JSON. 
 - goals: demonstrate how can AIS data from Perseus-M satellite can be accessed using API and UI
 - deliverables: a web-page with UI mapping AIS data, back-end for handling requests and demo requests to API to demonstrate each product's work.  
 - results: developed a decoder for typeA and typeB AIS messages, validation filters, statistics collection, writing data to JSON container, visualizing from Json to mapbox, mapbox clustering
 - http://earthimages.info/aismvp
- https://github.com/akudrya/AIS/tree/master/server-static/class%20A%2BB%20decoder
- https://github.com/akudrya/AIS/tree/master/server-static

4. Dynamic API - $2000
 - project description: R&D of system for collecting data from receining stations and giving API immidiate access to it.
 - goals: check feasibility and developm MVP for collecting AIS data directly from receivers and immidiately provide it in the API
 - deliverables: system for collecting AIS data from recievers and storing it in the API server.

** # 3 and 4 are tied to sucessful operations of Perseus-M satellites and sucessful completion of #2.

##Deliverables

### Week 1 (February 16-20):
- Market research 
  - [x] Pdf explaining what products can be launched from the API for small to big players. Here I'll give examples of data to be delivered, pricing framework, how data access going to be organized. (by Monday) https://github.com/akudrya/AIS/blob/master/s-AIS%20market%20research.pdf

- Imagery prototype
  - [x] Plan how to integrate AIS + satellite imagery data: I will implement matching vessels' coordinates and label satellite images with AIS data. I expect to have an issue with time synchronization. At least I will show approximately what vessels are on the photographed area. This is an integration with images themselves. - https://github.com/akudrya/AIS/blob/master/Landsat%20Project/Use%20Cases/AIS%2BLandsat%20-%20current%20state%2003:11.pdf
  - [x] Implement an access to satellite images automatically. - I've launched Landsat Metadata API. - https://github.com/akudrya/AIS/blob/master/Landsat%20Project/APIIntegration/app.js
  - [x] AIS + satellite imagery use cases. I'll make both slides and an online map using Mapbox where by clicking on a certain point a user can see a satellite image labeled with AIS data and with highlighted signs of sought-for types of activities. At first it will be a static picture for each use case. -  https://github.com/akudrya/AIS/blob/master/Landsat%20Project/Use%20Cases/Use%20Cases.pdf
  - [x] Plan high-level architechture of the system: platform, software, language, access modes - https://github.com/akudrya/AIS/blob/master/Landsat%20Project/Use%20Cases/Landsat%20use%20cases%2003:17.pdf

### Week 2 (February 23-27):
- Imagery prototype - Demo API for AIS+Satellite imagery product. 
  - [x] product specification: use cases, modes of work design - https://github.com/akudrya/AIS/blob/master/Landsat%20Project/Use%20Cases/AIS%2BLandsat%20-%20current%20state%2003:16.pdf
  - [x] back-end - https://github.com/akudrya/AIS/blob/master/Landsat%20Project/LandsatSearchVer1/js/app.js
  
### Week 3 (March 2-6):
 - Imagery prototype - Demo API for AIS+Satellite imagery product. 
  - [x] front-end - https://github.com/akudrya/AIS/blob/master/Landsat%20Project/LandsatSearchVer1/index.html
  - [x] tested demo requests - https://github.com/AstroDigital/AIS/issues/3
  - [x] documentation - https://github.com/akudrya/AIS/blob/master/Landsat%20Project/Use%20Cases/Landsat%20use%20cases%2003:17.pdf
  - [x] report - report on reseach articles - https://github.com/akudrya/AIS/blob/master/Landsat%20Project/Use%20Cases/Tracking%20vessels.pdf
  
 ### Week 4 (March 9-13):
- Demo API 
  - [x] Create back-end of the API on PHP to handle conditional requests like coordinates, name and MMSI filtering. - https://github.com/akudrya/AIS/blob/master/server-static/server.js
  - [x] Design sample requests to demonstrate API's work for selected types of products. So that you'll have text strings to be launched in web browser to demonstrate what data will be provided in JSON container. - http://54.153.113.251:8080/api/ais/mmsi/229166000

 ### Week 5 (March 16-20):
 - Demo API implementation + reporting
  - [x] Integrate more complex logic of showing data in Mapbox UI. Currently I've only labeled but all points from a sample dataset, filtered repeated dots and added representation of vessel's direction. - Processing JSON to collect all the records
  - [ ] Launch AWS virtual machine (currently I use my own web hosting Bluehost).
  - [ ] Migrate all the data+API back-end
  - [ ] a  report what I've done, next steps, problems and opportunities.
  - [ ] API documentation. 
  - [x] Plan of further development

- Dynamic API
 - [x] product specification: use cases, modes of work design
 - [x] research of how to integrate API with data received from the satellite 

 ### Week 5 (March 23-27):
- Dynamic API
  - front-end
  - back-end
  - tested demo requests
 
 ### Week 6 (March 30 - April 3):
- Dynamic API
  - beta tests
  - making edits, corrections
  - documentation
  - report 
  - final presentation of the first iteration
