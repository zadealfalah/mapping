# mapping
Interactive Shortest Path Calculator

## Table of Contents
* [General Info](#general-info)
* [To Do](#to-do)

## General Info
This notebook uses OpenCV and Dijkstra's to allow a user to interactively select possible stops (called points of interest or POIs) within an image and plot paths between them.  OpenCV is used to allow the user to see the full image and select where they would like to stop with a simple left mouse click.  Once they've selected all their possible stops, they issue one right mouse click and then Dijkstra's is used to calculate the shortest distance between each POI.  

The [mapping](https://github.com/zadealfalah/mapping/blob/main/mapping.ipynb) notebook contains all the code used as well as a simple example on a maze.

## To Do
- Error handling for when a path is not possible to complete
<<<<<<< Updated upstream
- Label points e.g. 'Start', 1, 2, ... , 'End'?  Could have 'End' denoted with a RMB, 'Start' by the first LMB.  May take up a lot of space on img.
=======
- Finalize decision on line width, colors, etc
- Edge detection to take and transform new images into ones the code can handle
>>>>>>> Stashed changes
