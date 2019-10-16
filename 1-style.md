## Part 1: Style

<!-- this needs to be revised to work off of pregenerated tiles -->

### Goal

Create a map style to display the points in your dataset as circles on the map.

### Instructions

#### Connect to the Atlas Flyaway Kit

Connect to the Atlas router's offline wireless network on a wifi-enabled laptop:
- network name (SSID): `flyaway-router` (or `flyaway-router-5G`)
- password: `nullisland`

Once connected to the network, navigate to http://192.168.1.2:2999/signin in your laptop's web browser and sign in with the following credentials:
- user: `atlas-user`
- password: `nullisland`

You should now see the main Atlas dashboard:
![](assets/images/atlas-dashboard.png)


#### Start a new style from a template:
- Navigate to the Atlas Studio Styles page at http://192.168.1.2:2999/studio
- Click "More options" to create a new style
- Choose one of the templates to start from, and click the "Create" button to start editing the style
- You should now be in the Studio map editor interface. At the top of the page, you'll see the title of your style (it will default to your template's title). Click the pencil icon to rename your style to something that will identify it as yours, e.g. "vakila-dark"


#### Create a new style layer:
- Click the "+" button in the upper left corner to add a new layer. You should now see the "Select data" panel.
- Scroll down in the data sources list until you find the Dataset you created. Click the Dataset name, then click the layer name that appears below.  
- You should now see your Dataset selected as the layer Source, and `Circle` should be automatically selected as the layer Type.

#### Style your layer
- Move to the "Style" panel by clicking the "Style" tab at the top of the panel (next to "Select Data" tab).
- Edit the style values to customize how your circles look. Try playing with any of these:
  - Radius: make the circles bigger/smaller
  - Color: change the circle color
  - Opacity: make the circles transparent
  - Stroke width: give the circles a border
  - Stroke color: change the border color
- Once you've styled your new custom layer, feel free to play around with the rest of the layers in the template. Click on a layer in the left sidebar to select it, then adjust the style properties however you wish.
- When you're happy with how your map looks (or when you're out of time!), click the "Publish..." button in the upper right corner to publish your map style so it can be used in a web page (our next activity!).

### Next step

[Part 2](./part-josm-edit.md)
