# Crag Route Viewer

Interactive WebGL point-cloud viewer for exploring a LiDAR scan, tracing climbing routes, and saving route projects.

## Run it

Open `index.html` in a modern browser. Internet access is required the first time it loads, to retrieve the Three.js library.

## Use it

1. Use **Load XYZ scan** to choose a Faro-style eight-column XYZ file or a six-column XYZ + RGB file.
2. Drag to orbit, scroll to zoom, and hover to see WGS84 coordinates based on the configured origin.
3. Select **Draw route** and click points to trace a red route. Finish the route, then start another to preserve the previous route.
4. Enter a project filename and select **Save project** to save the current view and routes as JSON. Use **Open project** to restore them after loading the same scan.

 
There is a sample of a lidar scan of a famous climbing crag Dinas y Gromlech in Llanberis Pass, Wales.
To load the raw Lidar file unzip the file scan010_zoomed_selected+rows.zip, then select Load XYZ Scan and load the .xyz file. This will need to be rotated and zoomed in for the correct orientation.
To see a saved edited version of this file with routes added select Open Project and locate the file crag-routes.json. 
This will display the crag in the corect orinetation with two example climbing routes shown in red.
The default coordinate conversion uses latitude `53.09083601367916` and longitude `-4.049058389140163`, assuming local X is metres east and local Y is metres north.
