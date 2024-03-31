# mapping
Interactive Shortest Path Calculator

## Table of Contents
* [General Info](#general-info)
* [Examples](#examples)
* [To Do](#to-do)

## General Info
This notebook uses OpenCV and Dijkstra's to allow a user to interactively select possible stops (called points of interest or POIs) within an image and plot paths between them.  OpenCV is used to allow the user to see the full image and select where they would like to stop with a simple left mouse click.  Once they've selected all their possible stops, they issue one right mouse click and then Dijkstra's is used to calculate the shortest distance between each POI.  

The [mapping](https://github.com/zadealfalah/mapping/blob/main/mapping.ipynb) notebook contains all the code used as well as a simple example on a maze.

## Examples
Below we can see two examples of this program.  The first is a simple map where we start at the top left and exit at the bottom left following the shortest calculated path.

![Simple Example Start](/examples/example_map_1_start.png)
![Simple Example Complete](/examples/example_map_1_complete.png)

Secondly we can see an example of multiple input points of interest (POIs) to stop at.  The program finds the shortest path between each point of interest in ascending order starting at point 0.  These POIs were selected via mouse cursor.  It is currently set to display the resulting paths piece-by-piece.

![Multistage Example Start](/examples/example_map_1_multistage_start.png)
![Multistage Example Complete](/examples/example_map_1_multistage_complete_pieces.png)

## To Do
- Deploy on AWS for others to use
- Error handling for when a path is not possible to complete e.g. if map had a square in it
- Finalize decision on line width, colors, etc
- Edge detection to take and transform new images into ones the code can handle
- Add further examples, include those with actual roads