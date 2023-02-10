---
title: TNFS
publishDate: 2023-02-09 00:00:00
img: /assets/tnfs.png
img_alt: Telecom Nancy File System
description: |
  A peer-to-peer hypermedia protocol implementation in C, based on IPFS
tags:
  - C
  - IPFS
  - Networks
---
# Telecom Nancy File System

Le projet est disponible sur [GitHub](https://github.com/lorisalx/tnfs).

TNFS (Telecom Nancy File System) est un projet développé par un groupe de trois étudiants à Telecom Nancy. Il s’agit d’une implémentation du protocole InterPlanetary File System ([IPFS](https://ipfs.tech/)), qui vise à créer un système de fichiers décentralisé et distribué. TNFS utilise la technologie peer-to-peer pour permettre aux utilisateurs de partager et d’accéder aux fichiers sans avoir besoin d’un serveur central ou d’un point de contrôle.

### Technologies

Ce projet a été réalisé en C.

### Fonctionnalités
#### Adressage de contenu
Nous avons mis en œuvre une version personnalisée de CID (Content Identifier) pour assurer l’intégrité des fichiers. Cette version utilise l’encodage Base32 et les algorithmes de hachage SHA-256, et est composée par programmation. Le CID est composé d’un préfixe indiquant l’encodage utilisé, suivi de caractères hexadécimaux représentant la version du CID, l’algorithme de hachage, la taille de hachage et le hachage lui-même.

#### Fractionnement des blocs
Le système utilise IPFS (InterPlanetary File System) et il a une fonctionnalité appelée "division par blocs" où les gros fichiers sont divisés en plusieurs blocs de 256 kilo-octets, permettant un transit plus rapide entre pairs et une décentralisation facile. Chaque bloc a une structure contenant le nom du fichier, le nombre de liens, le CID des liens, les données et la taille. Le bloc parent contient également le nom du fichier original et la liste des ID de tous les blocs contenant les données du fichier original. Ce CID est ce qui est transmis à l’utilisateur lors de l’ajout d’un fichier dans TNFS.

#### Échanges de réseaux
Nous avons mis en œuvre une version de base des échanges réseau utilisant le langage de programmation C, par opposition à l’utilisation de l’algorithme Kademlia plus avancé qui est utilisé dans IPFS.