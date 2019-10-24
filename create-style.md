## Style

<!-- this needs to be revised to work off of pregenerated tiles -->

### Goal

Create a custom map style that includes a layer with data from a given tileset.

### Instructions

#### Connect to the Atlas Flyaway Kit

Connect to the Atlas router's offline wireless network on a wifi-enabled laptop:
- network name (SSID): `atlaskit`
- password: `B!4st0ff`

Once connected to the network, navigate to http://192.168.1.100:2999/signin in your laptop's web browser and sign in with the following credentials:
- user: `atlas-user`
- password: `password`

You should now see the main Atlas dashboard:
![](assets/images/atlas-dashboard.png)


#### Start a new style from a template:
- Navigate to the Atlas Studio Styles page at http://192.168.1.100:2999/studio
- Click "More options" to create a new style
- Choose the "Satellite Streets" templates to start from, and click the "Create" button to start editing the style
- You should now be in the Studio map editor interface. At the top of the page, you'll see the title of your style (it will default to your template's title). Click the pencil icon to rename your style to something that will identify it as yours, e.g. "mikel-satellite-streets"
  - We are running a beta version of Atlas and there is a bug! Publishing will not work at this point. But it is simple to fix. Reload the page. Now continue.
- Experiment with changing the existing layers in the template. Click on a layer in the left sidebar to select it, then adjust the style properties however you wish. For example, try changing the color of some layers.


#### Create a new layer:
- Click the "+" button in the upper left corner to add a new layer. You should now see the "Select data" panel.
- Scroll down in the data sources list until you find the Tileset `Mapbox Boundaries Admin 3`. Click the Tileset name, then click the layer `boundaries_admin_3` that appears below.  
- You should now see the `boundaries-admin-3` Tileset selected as the layer Source, and `Fill` should be automatically selected as the layer Type (because Studio has detected that the data contains polygons). Change Type to `Line`

#### Style your layer
- Move to the "Style" panel by clicking the "Style" tab at the top of the panel (next to "Select Data" tab).
- Edit the style values to customize how your layer looks. Try playing with any of these:
  - Color: change the line color
  - Width: give the line a border

- When you're happy with how your map looks (or when you're out of time!), click the "Publish..." button in the upper right corner to publish your map style so other users and applications can access it. The "Compare" visualization shows the changes you've made compared to the original (template) style.

#### Add imagery layer:
Because of size constraints, Atlas comes with global satellite only to zoom level 12. We have added higher zoom tilesets on this field kit for Puerto Rico and San Juan.
- Again click the "+" button in the upper left corner to add a new layer. Scroll down to select `puertorico-satellite-14`. The layer Type `Raster` will automatically be selected for the layer `atlas-user-puertorico-satellite-14`
- In the Layers panel, drag the layer almost all the way down to the bottom, just above `mapbox-mapbox-satellite`
- Repeat the same with `sanjuan-satellite-17`, and drag to just above `atlas-user-puertorico-satellite-14`
- "Publish..." again

### Next step

[Part 2](./kepler.md)
