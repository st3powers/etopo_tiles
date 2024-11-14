# elev_tiles

Used gdal to wrap into mercator coordinate system
On windows desktop, used the OSGeo4W shell (not command prompt or powershell, which were having problems finding gdal).
Cannot recall if gdal was set up when installing OSGeo4W, or if gdal had to be set up separately.
So once gdal is installed and environment variables are set, the gdal functions should work from the command prompt too, but could not get this to work on the windows desktop. So- OSGeo4W shell instead. 

Yet on windows notebook, gdal functions did in fact work from common prompt on 2024 Nov 14. Strange.

Converted etopo projection to mercator using the belo (requires gdal install)(this worked on windows desktop on 2024 Nov 14)...
gdalwarp -t_srs EPSG:3857 ETOPO_2022_v1_60s_N90W180_surface.tif ETOPO_2022_v1_60s_N90W180_surface_mercator.tif

Use this to check for gdal functionality and file details...
gdalinfo ETOPO_2022_v1_60s_N90W180_surface.tif
