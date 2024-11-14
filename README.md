# elev_tiles

Used gdal to wrap into mercator coordinate system
On windows desktop, successfully used the OSGeo4W shell (not command prompt or powershell, which were having problems finding gdal) on @024 Nov 14.
Cannot recall if gdal was set up when installing OSGeo4W, or if gdal had to be set up separately.

On windows notebook, gdal functions did work from command prompt on 2024 Nov 14.

Back on windows desktop, after resetting environment variables, the gdal functions worked from the command prompt. But revert OSGeo4W shell if having problems getting gdal functions to work from command prompt. 

Convert etopo projection to mercator tif using the below (requires gdal install)(this worked on windows desktop on 2024 Nov 14)...
gdalwarp -t_srs EPSG:3857 ETOPO_2022_v1_60s_N90W180_surface.tif ETOPO_2022_v1_60s_N90W180_surface_mercator.tif

Use this to check for gdal functionality and file details...
gdalinfo ETOPO_2022_v1_60s_N90W180_surface.tif
