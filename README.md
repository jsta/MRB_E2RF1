# A Digital Hydrologic Network Supporting NAWQA MRB SPARROW Modeling--MRB_E2RF1

## Data source

[https://water.usgs.gov/GIS/dsdl/mrb_e2rf1.zip](https://water.usgs.gov/GIS/dsdl/mrb_e2rf1.zip)

[https://water.usgs.gov/GIS/metadata/usgswrd/XML/mrb_e2rf1.xml#stdorder](https://water.usgs.gov/GIS/metadata/usgswrd/XML/mrb_e2rf1.xml#stdorder)

## Make it modern...

```shell
e00conv mrb_e2rf1.e00 mrb_e2rf1_eeconv.e00

ogr2ogr -f "GPKG" -a_srs EPSG:5070 mrb_e2rf1.gpkg mrb_e2rf1_eeconv.e00
```
