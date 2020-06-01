# Tutorial: Spatial Analysis in Python

DATE: Wednesday, June 11 2020 - 18:00 UTC

AUDIENCE: Intermediate

INSTRUCTOR: Martin Bentley, Digital Geoscientist, [Agile](https://agilescientific.com/)

<!--### Video Stream:
<br>
<a href="" target="_blank">
    <img src="./youtube_logo.png" width=300 />
</a>-->

## Welcome
Welcome to a brief tutorial on using Python for spatial analysis. This is intended for people who are more or less comfortable with Python, in particular pandas and matplotlib. Spatial analysis and technology is a broad field, and it is almost certainly not possible to cover everything. This tutorial will focus on vector data (points, lines, and polygons).

As a short note, both ArcGIS and QGIS have their own flavour of Python (arcpy and pyqgis) available within the program. Since I am not sure what people have access to, this tutorial will take a third option and use geopandas.

## Set-up
If you wish to follow along with the live-coding then ensure that you have the following packages available:
* `jupyter` (the tutorial is run through a notebook)
* [`geopandas`](https://geopandas.org/install.html)
* [`mapclassify`](https://pysal.org/mapclassify/)
* [`contextily`](https://github.com/darribas/contextily)
* [`descartes`](https://pypi.python.org/pypi/descartes)
* [`matplotlib`](matplotlib.org/)
* [`geopy`](https://github.com/geopy/geopy)

It is recommended that these be installed in a new environment using anaconda. An `environment.yml` file is provided to facilitate this.

If you have conda installed, then `conda env create -f environment.yml` will set up an environment named `t20-wed-geo` in which everything should work. Type `conda activate t20-wed-geo` and you will be ready to roll.

The easiest way to get up and running for this tutorial will be to clone the [github repository](https://github.com/mtb-za/transform-2020-spatial-in-python/). Note that some of the data files are zipped. These can be left as they are.

Alternatively, a binder is available: [![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/mtb-za/transform-2020-spatial-in-python/master) This will let you run it all in a browser without installing anything. It may take some time to initialise, so if you want to go with this option, it might be good to arrive a little bit early to set it up.

## Other sessions

If you are interested in additional spatially-themed sessions specifically, the following may be of interest:
* [Spatial data analytics with geostatspy](https://transform2020.sched.com/event/cD0W/tutorial-open-source-spatial-data-analytics-in-python-with-geostatspy) (Already happened.)
* [Scattered points to gridded products using verde](https://transform2020.sched.com/event/c7KE/tutorial-from-scattered-data-to-gridded-products-using-verde)
* [Geologic image processing with Python](https://transform2020.sched.com/event/cD5T/tutorial-geologic-image-processing-with-python)

All session details are available [here](https://transform2020.sched.com/).
