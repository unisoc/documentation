# About

UNISOC IoT Documentation was created by mkdocs.

If you want to generate html format document, please follow below steps.

## Install required packages

	pip install --upgrade pip	#upgrade pip to the latest version
	pip install mkdocs			#install the mkdocs package
	pip install mkdocs-material	#install the Material theme package

You can also look into the officail website of [mkdocs](https://www.mkdocs.org/) and [Merterial](https://squidfunk.github.io/mkdocs-material) for more details.

## Get the document sources

	git clone https://github.com/unisoc/documentation.git

## Build html docs

	cd documentation
	mkdocs build

The HTML documents will be generated under `site` directory in a few seconds.
