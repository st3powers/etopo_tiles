# elev_tiles

# Converted etopo projection to mercator using the below, requires gdal install
gdalwarp -t_srs EPSG:3857 ETOPO_2022_v1_60s_N90W180_surface.tif ETOPO_2022_v1_60s_N90W180_surface_mercator.tif

# use to check for gdal functionality and file details
gdalinfo ETOPO_2022_v1_60s_N90W180_surface.tif
