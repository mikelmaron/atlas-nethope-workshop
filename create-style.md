## Part 1: Style

<!-- this needs to be revised to work off of pregenerated tiles -->

### Goal

Create a custom map style that includes a layer with data from a given tileset.

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
- Experiment with changing the existing layers in the template. Click on a layer in the left sidebar to select it, then adjust the style properties however you wish. For example, try changing the color of some layers.


#### Create a new layer:
- Click the "+" button in the upper left corner to add a new layer. You should now see the "Select data" panel.
- Scroll down in the data sources list until you find the Tileset `drc-adm2`. Click the Tileset name, then click the layer name that appears below.  
- You should now see the `drc-adm2` Tileset selected as the layer Source, and `Fill` should be automatically selected as the layer Type (because Studio has detected that the data contains polygons).

#### Style your layer
- Move to the "Style" panel by clicking the "Style" tab at the top of the panel (next to "Select Data" tab).
- Edit the style values to customize how your layer looks. Try playing with any of these:
  - Color: change the polygon color
  - Opacity: make the polygons transparent
  - Stroke width: give the polygons a border
  - Stroke color: change the border color
- [optional] Try changing the layer type to "Symbol" and adding a Text field based on one of the Data fields in the source data (e.g. `ADM2_VIZ_NAME`).
- When you're happy with how your map looks (or when you're out of time!), click the "Publish..." button in the upper right corner to publish your map style so other users and applications can access it. The "Compare" visualization shows the changes you've made compared to the original (template) style.

### Next step

[Part 2](./part-josm-edit.md)
