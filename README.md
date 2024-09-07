Interactive Map Coordinate Selection with Variable Storage.

## Overview
This repository provides a Python-based tool utilizing ipyleaflet and ipywidgets to create an interactive map interface. Users can draw shapes (rectangles for ranges or points for specific coords) directly on the map and automatically store their coordinates in a variable (bounds).
This project MUST be opened and run within Jupyter Notebook.

## Purpose
This tool is ideal for developers needing to extract geographical coordinates through an intuitive map interface, eliminating the need to manually input latitude and longitude values. It is especially useful for projects requiring the definition of specific or range-based coordinates that can be stored programmatically.
This solution is simple yet highly customizable, allowing developers to adapt it easily by referring to the ipyleaflet and ipywidgets documentation. While I haven't included a browser widget in this version, the code is flexible enough to allow developers to integrate such functionality, along with additional features, as needed.
## Features
- Interactive Map Interface: The map is centered on specified coordinates and allows users to visually interact with it.
- Draw Shapes: Supports drawing rectangles and points to select areas or specific locations.
- Coordinate Storage: Selected coordinates are automatically saved to a variable (bounds) for easy use in other parts of your project.
- Manual Map Centering: The initial coordinates where the map is centered are manually defined, allowing full control over the map's starting point.
- Dynamic Coordinate Display: The selected shape's coordinates are dynamically displayed and updated with a simple button click (Get Coordinates).
- Customizable Widgets: Integration with ipywidgets allows additional customization and the use of various widgets for different functionalities.

## Use Cases
This tool is ideal for:

- Geospatial Analysis: Quickly selecting areas of interest on a map.
- Coordinate Ranges: Marking specific regions for map-based applications.
- Visual Data Selection: Easily selecting coordinates for satellite imagery analysis, location-based services, or other geographic data needs.

## How It Works
- Map Initialization: The map is centered on user-defined coordinates (Initial coordinates) using the ipyleaflet library.
- Drawing Controls: The map includes options to draw rectangles (to select regions) and points (to select specific locations).
- Event Handling: When a shape is drawn, its coordinates are saved to the global variable shape_coords.
- Coordinate Display: Upon clicking the "Get Coordinates" button, the selected shape's coordinates are displayed in a widget and saved to the bounds variable. This variable can then be utilized throughout your code for any purpose, offering flexibility for integration into any kind of project.
