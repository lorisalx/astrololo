---
title: POI
publishDate: 2023-02-09 00:00:00
img: /assets/poifr.png
img_alt: POI, une application web fullstack visant à favoriser la démocratie participative
description: |
  Application web de "Civic Tech"
tags:
  - Fullstack
  - Web
---
## POI
POI (Point of Interest) est une application qui permet aux utilisateurs de découvrir et de partager des points d'intérêt à travers le monde. L'application permet aux utilisateurs de créer des POI avec des informations telles que le nom, la description, l'emplacement, les mentions "j'aime" et une photo. Les utilisateurs peuvent également effectuer des recherches en utilisant des filtres tels que le nom, la localisation, le type et le nombre de mentions "j'aime".

### Technologies
POI est développé à l'aide des technologies suivantes :
* [VueJS](https://vuejs.org/)
* [TailwindCSS](https://tailwindcss.com/)
* [FastAPI](https://fastapi.tiangolo.com/)
* [PostgreSQL](https://www.postgresql.org/)
* [Mapbox](https://www.mapbox.com/)

### Fonctionnalités

Lorsqu'un utilisateur arrive sur la page d'accueil de POI, il peut soit s'authentifier, soit consulter les POI déjà recensées. Sur la page de recherche, il peut consulter les POI en utilisant des filtres tels que le nom, la localisation, le type et le nombre de mentions "j'aime". L'utilisateur peut également consulter les POI les plus populaires du moment via la section "Tendances".

![Recherche](/assets/poirecherche.png)

Lorsqu'un utilisateur clique sur un POI, il accède à la page de profil du POI, où il peut consulter diverses informations telles que le nom, la description, l'emplacement, les mentions "j'aime" et une carte interactive. Pour avoir accès à plus de fonctionnalités telles que la création de POI, laisser des mentions "j'aime" et consulter une carte de France interactive, l'utilisateur doit se créer un compte et se connecter. L'utilisateur peut alors créer et modifier ses propres POI en donnant des informations telles que le nom, la description, le type et la localisation. Les autres utilisateurs peuvent ensuite donner des mentions "j'aime" sur le POI créé.

La fonctionnalité principale de POI est l'accès à une carte de France interactive, qui contient l'ensemble des POI recensés par tous les membres du site. L'utilisateur peut cliquer sur un marqueur sur la carte pour accéder aux informations du POI.

![Carte](/assets/poicartehome.png)