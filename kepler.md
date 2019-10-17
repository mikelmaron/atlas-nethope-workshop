## Visualize Data in Kepler

### Goal

Build and share two different custom interactive visualizations in Kepler from a single CSV dataset

### Requirements

Kepler works mainly on CSV data. For this lesson, we use [CSV data on violent incidents in Kivu](
https://github.com/OSU-Battelle-Center/DRC-Ebola-Conflict/blob/master/Data/kivu_security.csv) complied by the [Kivu Security Tracker](https://github.com/OSU-Battelle-Center/DRC-Ebola-Conflict/wiki/Dataset:-Violent-conflict-in-the-region) (A copy of the CSV file is available here at [data/kivu_security.csv](./data/kivu_security.csv).)

### Instructions

#### Launch Kepler with your data
Kepler.gl is a powerful and easy to use open source geospatial analysis tool for large-scale data sets. There is a link to open Kepler on the main page of Atlas, or directly at http://192.168.1.2:2999/kepler.gl


First, you will be prompted to upload data. Locate `kivu_security.csv` and upload.
![](assets/images/kepler-start.png)



#### Points visualization

Kepler will immediately create a simple Point visualization with the data set.
![](assets/images/kepler-points.png)

Open the "Points" visualization panel, click the color box under "Fill Color", and select another color for the points.
![](assets/images/kepler-fillcolor.png)

Open additional color options by clicking the "..." to the right of "Fill Color". Then click the box below "Color Based On", and select "Severity Rating". Kepler will apply a palette which increases brightness with the severity of the incident.
![](assets/images/kepler-severity.png)


Next apply a filter. Click the "Filters" panel, then "+ Add Filter". Click "Select a field", and select "severity_rating". Adjust the range below to filter out low severity incidents.
![](assets/images/kepler-filter.png)


Finally, adjust what fields are displayed when hovering over a point. Click the "Interactions" panel, and "x" off the "Latitude" and "Longitude" fields. Click elsewhere in the box and select "severity_rating", and "0/name".
![](assets/images/kepler-interaction.png)

#### Hexbin visualization

Before creating the second visualization, return to the "Filters" panel, and delete the filter.


Go back to the "Layers" panel, and under "Basic", click the visualization type dialog, and select "Hexbin". Also click the name of the Layer, and rename it from "Point" to "Hexbin". Hexbin will aggregate all points within a hexagonal tile.
![](assets/images/kepler-hexbin.png)

Change the "Radius" to 10, and "x" out the "Color based on" selection so that it is "Point Count". The brighter the color, the more incidents occurred in that hexbin


To create a 3D view of the hexbins, select "3D Map" on the upper right side, and also "Show Legend". Enable "Height" in the "Layers" panel, and adjust "Elevation Scale" to 30.
![](assets/images/kepler-3d.png)

#### Compare visualizations

Add and recreate the original Points layer above, and then enable "Switch to dual map view" with the button in the upper right. Click the layers button in the upper right of each panel to "Show layer panel" and choose which layers are visible in each panel. Select "Hexbin" in one and "Point" in another, to explore both views at once.
![](assets/images/kepler-dual.png)

#### Change the base map

In the left hand panel, click the "Base map" tab, and click "+ Add Map Style". In another tab, find the Satellite style from the [Studio Styles page](http://192.168.1.2:2999/studio/), and click "Share & Use". Switch to the "Use" tab and copy the access token, and then the style URL. Paste these into the "Add Custom Mapbox Style" dialog in Kepler.
![](assets/images/kepler-custom.png)

![](assets/images/kepler-satellite.png)

#### Finalize and share the visualization

Finally Click "Share", then "Export Map". Make sure "json" is selected for the "Map format", then click "Export". This will trigger a download of "keplergl.json".
![](assets/images/kepler-export.png)

This file contains both the data and styling to recreate the visualization. You can share this json file with a colleague by email or flash disk, and they can upload to kepler to see your visualization.

To test this, reload your browser, and you will see the original "Add Data to Map" dialog. Find the json file you downloaded, and upload. Your visualization will be recreated entirely.
