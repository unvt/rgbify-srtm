# rgbify-srtm
Rgbifying SRTM dem

# Procedure

1. Download srtm data (1 sec, V3) and save it into the src directory.

2. Use docker or podman if you do not have gdal_merge.py or rasterio command installed.

```
 docker run -it --rm -v ${PWD}:/data unvt/rgbify-node
```

3. Run the following commands:

```
node index4merge-re.js
node index4rgb.js
```

If there is the file in merge/mbtiles folder, it skips the conversion.

# Other 
This is originally developed at https://github.com/ubukawa/srtm-rgbify


