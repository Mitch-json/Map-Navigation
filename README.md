# A* Pathfinding for Real-World Navigation Using OpenStreetMap Data

This repository contains a complete implementation of a real-world navigation system using the A* search algorithm applied to geospatial road networks extracted from **OpenStreetMap (OSM)**.
The project demonstrates how classical graph search algorithms can be applied to real geographic data, and compares their performance to modern navigation tools such as Google Maps.

The work emphasizes algorithmic design, geospatial data processing, heuristic analysis, and practical graph-based modeling using real map networks.

## Core Concepts & Techniques

#### 1. Geospatial Graph Modeling (OSMnx)

We download and construct detailed drivable road networks from OSM using OSMnx, converting them into NetworkX graph structures.
This provides the foundation for all routing operations.

#### 2. A* Search Algorithm (Heuristic Pathfinding)
We implement the A* search algorithm from scratch:

* Uses straight-line (Euclidean) distance as the admissible heuristic
* Ensures optimal shortest-path discovery
* Explores nodes efficiently by balancing cost so far and estimated cost to goal
This demonstrates how classical AI search techniques operate on large, real-world maps.

#### 3. Route Planning & Comparison

The system computes: 
* Shortest paths between two user-defined points
* Routes based on both GPS coordinates and IP-derived locations
* Side-by-side comparisons with Google Maps routing results

#### 4. Visualization & Mapping

The project generates clear visual outputs that include:
* The extracted road network
* The A*-computed route
* Start and destination markers
* Overlays comparing A* results with Google Maps routing

These visualizations make it easy to understand the geographical behavior of the algorithm.

#### 5. Location Accuracy Analysis

The project evaluates the accuracy of IP-derived location estimates versus actual GPS coordinates.  
It demonstrates how inaccuracies in IP geolocation can influence routing results and affect path quality.
