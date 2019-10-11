## Part X: Process Imagery on Atlas

### Goal

### Requirements

### Instructions


* loading data onto Atlas (scp)
* Rasterio
  * https://github.com/mapbox/rio-mbtiles
* copying into tile directory
* Here is some UAV imagery of Kinshasa from OAM
% rio mbtiles --src-nodata 0 --resampling bilinear --zoom-levels 13..20 -f PNG 5b1e6fd42b6a08001185f7c0.tif -o /tmp/5b1e6fd.mbtiles

PNG format because JPEG doesn't support transparency
and --src-nodata 0 because the source file doesn't carry a nodata value
bilinear looks good and is fast enough

Build a style using a satellite image


Imagery Advanced Topics?
Dealing with nodata



### Next step
