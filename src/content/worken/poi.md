---
title: POI
publishDate: 2023-02-09 00:00:00
img: /assets/poi.png
img_alt: POI, a fullstack web application to help democracy
description: |
  Participatory democracy web application 
tags:
  - Fullstack
  - Web
---
## POI

POI (Point of Interest) is an application that allows users to discover and share points of interest around the world. The application allows users to create POIs with information such as name, description, location, likes, and a photo. Users can also perform searches using filters such as name, location, type, and number of likes.

### Technologies
POI is developed using the following technologies:

* [VueJS](https://vuejs.org/)
* [TailwindCSS](https://tailwindcss.com/)
* [FastAPI](https://fastapi.tiangolo.com/)
* [PostgreSQL](https://www.postgresql.org/)
* [Mapbox](https://www.mapbox.com/)

### Features
When a user arrives at the POI homepage, they can either log in or view previously recorded POIs. On the search page, they can view POIs using filters such as name, location, type, and number of likes. The user can also view the most popular POIs of the moment through the "Trends" section.

![Trends](/assets/poirecherche.png)

When a user clicks on a POI, they are taken to the POI profile page, where they can view various information such as name, description, location, likes, and an interactive map. To access more features such as creating POIs, leaving likes, and viewing an interactive map of France, the user must create an account and log in. The user can then create and modify their own POIs by providing information such as name, description, type, and location. Other users can then give likes on the created POI.

The main feature of POI is access to an interactive map of France, which contains all the POIs recorded by all site members. The user can click on a marker on the map to access the POI information.

![Map](/assets/poicartehome.png)