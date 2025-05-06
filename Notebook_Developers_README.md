# Creating Exploratory Notebooks For Your Dataset
This repository will be used by MSD-LIVE's Jupyter Notebook Services to provide the default notebooks that will be available to a user when they click the "Explore Data" icon on your dataset's landing page.  These notebooks will enable users to visualize, interact with, and/or subset your data for subsequent download.  See [this help page](https://msdlive.org/sb/help/resources/quick-guides/jupyter-notebooks) describing this feature.

In order to work with MSD-LIVE's Jupyter Notebook services, you will need to configure the following three types of information:

1) README.md - contains instructions for your users
2) requirements.txt - contains the python dependencies for your notebooks
3) notebooks - one or more notebooks that can be used to visualize, explore, and subset your dataset


## Note:
* Everything in your repo will be cloned into the user's home folder when the notebook is spawned
* If this repo contains large or many files it will take longer for the notebook to launch

The steps for creating these files are provided in the sections below.

## **Step 1:**  Create notebook repository
* Make sure that you have created a new repository in your GitHub organization from the following template repository:  <https://github.com/MSD-LIVE/template-dataset-jupyter-notebook>
* Once created, make sure that you copy the repository URL and paste it into your dataset's upload form on the MSD-LIVE web site.

## **Step 2:** Edit the README.md file
The README.md file contains the instructions your user will see when they first explore your data.  This file should summarize each notebook you provide and explain its purpose. 

## **Step 3:** Create your *.ipynb notebook files
* Your dataset's data will be mounted into the notebook at $DATA_DIR (or /data, also symlinked under the user's home dir at ~/data)
* All file paths used in the notebook must be relative to $DATA_DIR
* The $DATA_DIR folder is READ-ONLY.
* Notebooks should have as the first cell installing dependencies. See examples of installing dependencies and accessing data from $DATA_DIR in: 
  * Python kernels: [example_python.ipynb](/example_python.ipynb)
  * Julia kernels: [example_julia.ipynb](/example_julia.ipynb)
  * R kernels: [example_r.ipynb](/example_r.ipynb)

