---
layout: post
title: Working with lots of point data
---


This is a developing tutorial for working with massive amounts of location data. I think this type of work comes up most often with cellphone location data. Instead of using cell data, I am using [marine AIS vessel location data](http://marinecadastre.gov/ais/), from the U.S. Coast Guard. This data is perhaps not truely 'big', but one month takes up about 800 mb when zipped, and it takes arcGIS a long time to load (which might be a working definition of big data for GIS folks.) 

It stems from the very basic question - where should I go kayaking if I don't want to get run over or massively waked out by marine traffic in Puget Sound. 

## Convert data into a better format

The data arrives as a .gdb folder. Step one is to convert it to something more flexible. To do so, I use the built in tools QGIS has take a .gdb and save it both a .csv and and .geoJson. These files are big,but they are a start.

| data type     | size (GB)     | 
| ------------- |:-------------:| 
| ucompressed GDB      | 2.65 | 
| CSV     | 2.35      | 
| geoJSON |7.95      |


CSV can be easily read into pandas, Tableau, etc. I am exploring the uses geoJSON right now, but    
