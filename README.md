# DigitalNZ

Current version: [v1.0.0](https://github.com/GLAM-Workbench/digitalnz/releases/tag/v1.0.0)

Jupyter notebooks to work with data from DigitalNZ's API. For more information see the [DigitalNZ](https://glam-workbench.net/digitalnz/) section of the GLAM Workbench.

## Notebook topics

### Exploring the API

* [Build a DigitalNZ API search query](build_api_query.ipynb) – experiment with the DigitalNZ search API
* [Getting some top-level data from the DigitalNZ API](Top-level-data-in-DigitalNZ.ipynb) – poke around at the top-level of DigitalNZ, mainly using facets to generate some collection overviews and summaries

### Harvesting data

* [Harvest facet data from DigitalNZ](harvest_facet_data.ipynb) – explores what facets are available from the DigitalNZ API and demonstrates how to harvest data from them
* [Harvest data from Papers Past](Harvest-data-from-PapersPast.ipynb) – harvest large amounts of data from [Papers Past](https://paperspast.natlib.govt.nz/) (via DigitalNZ) for further analysis

### Tips and tricks

* [Select a random(ish) record from DigitalNZ](select_a_random_record.ipynb) – examines the available facets, then uses them to reduce the size of the results set until it's possible to select a random record
* [Find results by country in DigitalNZ](Results-by-country-in-DigitalNZ.ipynb) – find records relating to particular countries by searching for geocoded locations using bounding boxes

### Visualising collections

* [QueryPic DigitalNZ](querypic_papers_past.ipynb) – a web app to visualise searches in Papers Past over time
* [Visualise a search in Papers Past](Visualise-a-search-in-PapersPast.ipynb) – create a simple visualisation showing the distribution of a search over time and by newspaper
* [Papers Past newspapers in DigitalNZ](papers_past_newspapers.ipynb) – displays details of the Papers Past newspapers available through DigitalNZ
* [Visualising open collections in DigitalNZ](visualise_open_collections.ipynb) – assemble data relating to the `usage` status of collections and visualise the results in a suitably colourful burst of fireworks!

## Datasets

* [Summary of facets](https://github.com/GLAM-Workbench/digitalnz/blob/master/facets/facets.csv)
* Individual facets:
  * [collection.csv](https://github.com/GLAM-Workbench/digitalnz/blob/master/facets/category.csv)
  * [creator.csv](https://github.com/GLAM-Workbench/digitalnz/blob/master/facets/creator.csv)
  * [subject.csv](https://github.com/GLAM-Workbench/digitalnz/blob/master/facets/subject.csv)
  * [format.csv](https://github.com/GLAM-Workbench/digitalnz/blob/master/facets/format.csv)
  * [placename.csv](https://github.com/GLAM-Workbench/digitalnz/blob/master/facets/placename.csv)
  * [decade.csv](https://github.com/GLAM-Workbench/digitalnz/blob/master/facets/decade.csv)
  * [content_partner.csv](https://github.com/GLAM-Workbench/digitalnz/blob/master/facets/content_partner.csv)
  * [language.csv](https://github.com/GLAM-Workbench/digitalnz/blob/master/facets/language.csv)
  * [century.csv](https://github.com/GLAM-Workbench/digitalnz/blob/master/facets/century.csv)
  * [usage.csv](https://github.com/GLAM-Workbench/digitalnz/blob/master/facets/usage.csv)
  * [rights.csv](https://github.com/GLAM-Workbench/digitalnz/blob/master/facets/rights.csv)
  * [year.csv](https://github.com/GLAM-Workbench/digitalnz/blob/master/facets/year.csv)
  * [copyright.csv](https://github.com/GLAM-Workbench/digitalnz/blob/master/facets/copyright.csv)
  * [dc_type.csv](https://github.com/GLAM-Workbench/digitalnz/blob/master/facets/dc_type.csv)
  * [category.csv](https://github.com/GLAM-Workbench/digitalnz/blob/master/facets/category.csv)
  * [primary_collection.csv](https://github.com/GLAM-Workbench/digitalnz/blob/master/facets/primary_collection.csv)
* [collections_by_partner.csv](https://github.com/GLAM-Workbench/digitalnz/blob/master/facets/collections_by_partner.csv)
* [usage_by_collection_and_partner.csv](https://github.com/GLAM-Workbench/digitalnz/blob/master/facets/collections_by_partner.csv)

See the [GLAM Workbench for more details](https://glam-workbench.github.io/digitalnz/).


<!-- START RUN INFO -->


## Run these notebooks

There are a number of different ways to use these notebooks. Binder is quickest and easiest, but it doesn't save your data. I've listed the options below from easiest to most complicated (requiring more technical knowledge).

### Using Binder

[![Launch on Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/GLAM-Workbench/digitalnz/master/?urlpath=lab/tree/index.md)

Click on the button above to launch the notebooks in this repository using the [Binder](https://mybinder.org/) service (it might take a little while to load). This is a free service, but note that sessions will close if you stop using the notebooks, and no data will be saved. Make sure you download any changed notebooks or harvested data that you want to save.

See [Using Binder](https://glam-workbench.net/using-binder/) for more details.

### Using Reclaim Cloud

[![Launch on Reclaim Cloud](https://glam-workbench.github.io/images/launch-on-reclaim-cloud.svg)](https://app.my.reclaim.cloud/?manifest=https://raw.githubusercontent.com/GLAM-Workbench/digitalnz/master/reclaim-manifest.jps)

[Reclaim Cloud](https://reclaim.cloud/) is a paid hosting service, aimed particularly at supported digital scholarship in hte humanities. Unlike Binder, the environments you create on Reclaim Cloud will save your data – even if you switch them off! To run this repository on Reclaim Cloud for the first time:

* Create a [Reclaim Cloud](https://reclaim.cloud/) account and log in.
* Click on the button above to start the installation process.
* A dialogue box will ask you to set a password, this is used to limit access to your Jupyter installation.
* Sit back and wait for the installation to complete!
* Once the installation is finished click on the 'Open in Browser' button of your newly created environment (note that you might need to wait a few minutes before everything is ready).

See [Using Reclaim Cloud](https://glam-workbench.net/using-reclaim-cloud/) for more details.

### Using Docker

You can use Docker to run a pre-built computing environment on your own computer. It will set up everything you need to run the notebooks in this repository. This is free, but requires more technical knowledge – you'll have to install Docker on your computer, and be able to use the command line.

* Install [Docker Desktop](https://docs.docker.com/get-docker/).
* Create a new directory for this repository and open it from the command line.
* From the command line, run the following command:  
  ```
  docker run -p 8888:8888 --name {{ cookiecutter.repository_name }} -v "$PWD":/home/jovyan/work quay.io/glamworkbench/digitalnz repo2docker-entrypoint jupyter lab --ip 0.0.0.0 --NotebookApp.token='' --LabApp.default_url='/lab/tree/index.ipynb'
  ```
* It will take a while to download and configure the Docker image. Once it's ready you'll see a message saying that Jupyter Notebook is running.
* Point your web browser to `http://127.0.0.1:8888`

See [Using Docker](https://glam-workbench.net/using-docker/) for more details.

### Setting up on your own computer

If you know your way around the command line and are comfortable installing software, you might want to set up your own computer to run these notebooks.

Assuming you have recent versions of Python and Git installed, the steps might be something like:

* Create a virtual environment, eg: `python -m venv digitalnz`
* Open the new directory" `cd digitalnz`
* Activate the environment `source bin/activate`
* Clone the repository: `git clone https://github.com/GLAM-Workbench/digitalnz.git notebooks`
* Open the new `notebooks` directory: `cd notebooks`
* Install the necessary Python packages: `pip install -r requirements.txt`
* Run Jupyter: `jupyter lab`

See the [GLAM Workbench for [more details](https://glam-workbench.net/getting-started/#using-python-on-your-own-computer.

<!-- END RUN INFO -->

## Cite as

See the GLAM Workbench or [Zenodo](https://doi.org/10.5281/zenodo.3544729) for up-to-date citation details.

----

This repository is part of the [GLAM Workbench](https://glam-workbench.net/). If you think this project is worthwhile, you can become [a GitHub sponsor](https://github.com/sponsors/wragge?o=esb).
