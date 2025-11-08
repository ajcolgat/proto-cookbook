# Alex's Prototype Cookbook

<img src="thumbnails/thumbnail.png" alt="thumbnail" width="300"/>

[![nightly-build](https://github.com/ProjectPythia/cookbook-template/actions/workflows/nightly-build.yaml/badge.svg)](https://github.com/ProjectPythia/cookbook-template/actions/workflows/nightly-build.yaml)
[![Binder](https://binder.projectpythia.org/badge_logo.svg)](https://binder.projectpythia.org/v2/gh/ProjectPythia/cookbook-template/main?labpath=notebooks)
[![DOI](https://zenodo.org/badge/475509405.svg)](https://zenodo.org/badge/latestdoi/475509405)


This Project Pythia Cookbook covers working with gridded radar reflectivity data from GridRad. 

## Motivation

This notebook will show the beginning outline of this project and how it will be structured. It will go into detail as to the foundations for this project and show the dataset that I will be using. This outline will help me get a better idea on how to format the project and import the datasets. 

## Authors

[Alex Colgate](https://github.com/ajcolgat), [Amanda Maminimini](https://github.com/Amaminimini), [Alex Kramer](https://github.com/krameral), 
[Mark Warburg](https://github.com/Warburgm) 

### Contributors

<a href="https://github.com/ProjectPythia/cookbook-template/graphs/contributors">
  <img src="https://contrib.rocks/image?repo=ProjectPythia/cookbook-template" />
</a>

## Structure

This notebook is broken up into two sections: "Foundations" and "Example Workflows". 

### Foundations 

The foundational content includes the different synoptic environments in the Northeast U.S. we will be testing to look at the role of topography on different severe thunderstorm events, and information on the GridRad-Severe Version 4.2 dataset to read in and study gridded reflectivity analysis. 

### Example workflows 

Some example workflows include the gridradpy package to read in the GridRad data, in conjunction with xarray, netCDF4 and matplotlib. I will be importing reflectivity data from the GridRad package based on specific severe thunderstorm events we choose. Additionally, I will be importing some ERA5 hourly data to compare with the outputs from the GridRad-Severe data. 

## Running the Notebooks

You can either run the notebook using [Binder](https://binder.projectpythia.org/) or on your local machine.

### Running on Binder

The simplest way to interact with a Jupyter Notebook is through
[Binder](https://binder.projectpythia.org/), which enables the execution of a
[Jupyter Book](https://jupyterbook.org) in the cloud. The details of how this works are not
important for now. All you need to know is how to launch a Pythia
Cookbooks chapter via Binder. Simply navigate your mouse to
the top right corner of the book chapter you are viewing and click
on the rocket ship icon, (see figure below), and be sure to select
“launch Binder”. After a moment you should be presented with a
notebook that you can interact with. I.e. you’ll be able to execute
and even change the example programs. You’ll see that the code cells
have no output at first, until you execute them by pressing
{kbd}`Shift`\+{kbd}`Enter`. Complete details on how to interact with
a live Jupyter notebook are described in [Getting Started with
Jupyter](https://foundations.projectpythia.org/foundations/getting-started-jupyter).

Note, not all Cookbook chapters are executable. If you do not see
the rocket ship icon, such as on this page, you are not viewing an
executable book chapter.


### Running on Your Own Machine

If you are interested in running this material locally on your computer, you will need to follow this workflow:

1. Clone the `https://github.com/ProjectPythia/proto-cookbook` repository:

   ```bash
    git clone https://github.com/ProjectPythia/proto-cookbook.git
   ```

1. Move into the `proto-cookbook` directory
   ```bash
   cd proto-cookbook
   ```
1. Create and activate your conda environment from the `environment.yml` file
   ```bash
   conda env create -f environment.yml
   conda activate proto-cookbook
   ```
1. Move into the `notebooks` directory and start up Jupyterlab
   ```bash
   cd notebooks/
   jupyter lab
   ```
