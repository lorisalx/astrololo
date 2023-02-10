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
## Telecom Nancy File System

The project is available on [GitHub](https://github.com/lorisalx/tnfs).

TNFS (Telecom Nancy File System) is a project developed by a group of three students at Telecom Nancy. It is an implementation of the InterPlanetary File System ([IPFS](https://ipfs.tech/)) protocol, which aims to create a decentralized and distributed file system. TNFS utilizes peer-to-peer technology to enable users to share and access files without the need for a central server or point of control.
### Technologies

This project was developed in C.
#### Features

#### Content addressing
We have implemented a customized version of CID (Content Identifier) to ensure the integrity of files. This version uses Base32 encoding and SHA-256 hashing algorithms, and is composed programmatically. The CID is made up of a prefix character indicating the encoding used, followed by hexadecimal characters representing the CID version, hash algorithm, hash size, and the hash itself.

#### Bloc splitting
The system uses IPFS(InterPlanetary File System) and it has a feature called "block splitting" where large files are divided into multiple blocks of 256 kilo-bytes, allowing faster transit between peers and easy decentralization. Each block has a structure containing the file name, number of links, CID of links, data, and size. The parent block also contains the original file name and the list of CIDs of all the blocks containing the original file's data. This CID is what is transmitted to the user when adding a file to TNFS.

#### Network exchanges
We have implemented a basic version of network exchanges using C programming language, as opposed to utilizing the more advanced Kademlia algorithm which is used in IPFS.