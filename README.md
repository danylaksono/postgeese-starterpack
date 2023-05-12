# Postgeese-starterpack

## What's this

The following is a basic steps for setting up duckdb and it's spatial extension, [PostGEESE](https://duckdb.org/2023/04/28/spatial.html). This notebook can be used as starting point for building poor man's data lake (or to be precise, data 'pond') for geospatial data science analytics using DuckDB's latest [Spatial Extension](https://github.com/duckdblabs/duckdb_spatial). 

Credit to:
- [Mark Litwintschik](https://tech.marksblogg.com/duckdb-geospatial-gis.html), one of the very first articles discussing about the wonderful of DuckDB to the geospatial community
- [Mark Forrest](https://www.youtube.com/watch?v=ljzpm3Mrw-I) for the inspiration.
- [Wei-Meng Lee](https://towardsdatascience.com/running-sql-queries-in-jupyter-notebook-using-jupysql-duckdb-and-mysql-3c53fbe40f8d) for the examples on JupySQL

## How to use
- Download the data from [here](https://data.london.gov.uk/dataset/local-authority-maintained-trees), convert the CSV file to GeoJSON using QGIS. Name it `london-trees.geojson`. We can also use parquet, which is smaller in size. The spatial extension can also read CSV's using its GDAL driver ( see the docs for `st_read()` [here](https://duckdb.org/docs/extensions/spatial.html)). Change the code accordingly.
- Put the file in the same folder
- Fire up your Jupyter Notebook or upload to Google Colab
- Have fun!
