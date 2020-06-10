# Tutorial: Spatial Analysis in Python

DATE: Friday, June 12 2020 - 08:00 UTC

AUDIENCE: Intermediate

INSTRUCTOR: Martin Bentley, Digital Geoscientist, [Agile](https://agilescientific.com/)

Part of the [SoftwareUndergrounds](https://swu.ng) online conference, [TRANSFORM2020](https://transform2020.sched.com/).

### Video Stream:
<a href="https://www.youtube.com/watch?v=t5FjmDwwTnA" target="_blank">Direct link to the live stream.
</a>

## Welcome
Welcome to a brief tutorial on using Python for spatial analysis. This is intended for people who are more or less comfortable with Python, in particular pandas and matplotlib. Spatial analysis and technology is a broad field, and it is almost certainly not possible to cover everything. This tutorial will focus on vector data (points, lines, and polygons).

As a short note, both ArcGIS and QGIS have their own flavour of Python (arcpy and pyqgis) available within the program. Since I am not sure what people have access to, this tutorial will take a third option and use geopandas.

## Set-up
### Install-less (cloud) set-up
A [binder version](https://mybinder.org/v2/gh/mtb-za/transform-2020-spatial-in-python/master) of this repository is available. Clicking that link will let you run everything in a browser without installing anything. It may take some time to initialise, so if you want to go with this option, it might be good to arrive a little bit early to set it up. 

Because mybinder.org is a best-effort, free service, if there are many people attempting to use this service, it may be oversubscribed. If possible, it is recommended that you set up a local environment instead.

### Local set-up
The easiest way to get up and running for this tutorial will be to clone the [github repository](https://github.com/mtb-za/transform-2020-spatial-in-python/). Note that some of the files the data folder are zipped. These can be left as they are, unless you are particularly curious.

It is recommended that you use the Anaconda python distribution. Please see the end of this section for some help if you need to install this.

Once you have conda installed, navigate to the downloaded folder, and type `conda env create -f environment.yml` in the Anaconda prompt. This will set up an environment named `t20-fri-geo` in which everything should work. Type `conda activate t20-fri-geo`, followed by `jupyter notebook` and you will be ready to roll. This will open a page in your web browser - please make sure that you use either Firefox, Chrome or Edge.

If you are doing things manually, the minimal packages to install are the following along with their dependencies:
* `jupyter` (the tutorial is run through a notebook)
* [`geopandas`](https://geopandas.org/install.html)
* [`mapclassify`](https://pysal.org/mapclassify/)
* [`contextily`](https://github.com/darribas/contextily)
* [`descartes`](https://pypi.python.org/pypi/descartes)
* [`matplotlib`](matplotlib.org/)
* [`geopy`](https://github.com/geopy/geopy)

It is recommended that these be installed in a new environment using anaconda.

Additional set-up instructions in the form of videos for [Windows](https://youtu.be/FdatS_NKVrM) and [Linux](https://youtu.be/3ncwbHyZeAg), or as a [written guide](http://swu.ng/t20-python-setup) are available. Alternatively, please feel free to ask in the #t20-fri-geo channel in the [Slack group](swu.ng/slack).

## Other sessions

If you are interested in additional spatially-themed sessions specifically, the following may be of interest:
* [Spatial data analytics with geostatspy](https://transform2020.sched.com/event/cD0W/tutorial-open-source-spatial-data-analytics-in-python-with-geostatspy)
* [Scattered points to gridded products using verde](https://transform2020.sched.com/event/c7KE/tutorial-from-scattered-data-to-gridded-products-using-verde)
* [Geologic image processing with Python](https://transform2020.sched.com/event/cD5T/tutorial-geologic-image-processing-with-python)

All have already happened, but the recordings of the live streams are still available via the [Software Underground YouTube channel](https://www.youtube.com/channel/UCeDefhvz7znDo29iOmqU_9A).

