## Digitize Imagery in JOSM

### Goal

Configure JOSM to load an aerial imagery style hosted on Atlas

![Atlas Hosted Imagery for Digitizing in JOSM](assets/images/josm-editing.png)

### Requirements

- A computer connected to the flyaway-router network, with [JOSM](http://josm.openstreetmap.de) installed (you can download the local copy of [josm-tested.jar](./data/josm-tested.jar).
- An imagery style built in Atlas


### Instructions

First, get the `WTMS` integration endpoint for the style.

![Atlas Style Share](assets/images/style-share.png)

From the Atlas style page, click "Share", then switch to the "Use" tab.

![Atlas Integration URL](assets/images/share-integration-url.png)

In the Share dialog, click `Third Party`, and then `WMTS`. Copy the `Integration URL`.


![JOSM config](assets/images/josm-config.png)

Now open JOSM on your own computer. In JOSM, open the `Imagery Preferences` panel in `Preferences`. In the bottom right click the `WTMS` button.
* Paste the integration URL below `2. Enter Get Capabilities URL`.
* Select `Set default layer?`
* Click `3. Get layers`
* Below `Choose default layer`, only one layer will load. Select it.
* Below `4. Enter name for this layer`, give the layer a memorable name.
* Click `Ok`

Now you can use this imagery hosted on the Atlas Fly Away Kit for editing map data in JOSM. (In the `Imagery` menu, select the name of the layer you just created.)

Note: The Fly Away Kit may not be connected to the internet. So to download and upload OSM data, connect your laptop to another access point for data transfer. Then reconnect to the WIFI for the Fly Away Kit.

Happy Editing!
