<img src="https://raw.githubusercontent.com/ProjectPythiaCookbooks/radar-cookbook/main/thumbnail.png" alt="thumbnail" width="300"/>

# MSCAR Python Workshop

[![nightly-build](https://github.com/ProjectPythiaCookbooks/cookbook-template/actions/workflows/nightly-build.yaml/badge.svg)](https://github.com/ProjectPythiaCookbooks/cookbook-template/actions/workflows/nightly-build.yaml)
[![Binder](https://mybinder.org/badge_logo.svg)](https://aws-uswest2-binder.pangeo.io/v2/gh/mgrover1/mscar-python-workshop-2022/main?labpath=notebooks)


## Motivation

This material will be used to provide an overview of how to use Python for the atmospheric and climate sciences.

## Authors

[Max Grover](@mgrover1) [Zach Sherman](zssherman) [Scott Collis](@scollis) [Adam Theisen](@AdamTheisen)

### Contributors

<a href="https://github.com/mgrover1/mscar-python-workshop-2022/graphs/contributors">
  <img src="https://contrib.rocks/image?repo=mgrover1/mscar-python-workshop-2022" />
</a>

## Workshop Recording
The recording for this workshop can be found here!

[![MSCAR Python Workshop 2022](https://img.youtube.com/vi/aNeAtaJWA5M/0.jpg)](https://youtu.be/aNeAtaJWA5M)

## Structure

### Radar Data with Py-ART
Within this section, we cover the basics of Py-ART and apply it to a sample analysis workflow.

### Weather Observations with ACT
The Atmospheric data Community Toolkit (ACT) is a helpful tool when working with atmospheric observations! This portion will focus on reading, visualizing, and analyzing observational datasets from the Atmospheric Radiation Measurement user facility.

### Climate Analysis with Pangeo
Our last section covers how to use the Pangeo stack, specifically Intake-ESM, Xarray, and other components to inspect and visualize earth system model data.

## Running the Notebooks
You can either run the notebook using [Binder](https://mybinder.org/) or on your local machine.

### Using on the Pangeo Binder (**Recommended**)

#### 1. Make Sure You Have a Github Account
The first step is to make sure you have a Github Account.

Here is the link if you do have one already:
- [Github account creation link](https://github.com/join)

#### 2. Log into Pangeo Binder
Next, sign in and authenticate the Pangeo Binder, which is the platform we will use for the workshop:
- [Pangeo Binder Link](https://aws-uswest2-binder.pangeo.io)

The JupyterHub instance we use for this course is relatively small in memory and compute power (~10 GB of memory, 2 CPU cores). For more information about all of the open computational resrouces available within the Pangeo community, check out the [Pangeo Cloud](https://pangeo.io/cloud.html) documentation.

#### 3. Launch our Environment
Now that we have our authentication set up, we can access our content!

Use the following link to launch into the binder:
- [Binder Link](https://aws-uswest2-binder.pangeo.io/v2/gh/mgrover1/mscar-python-workshop-2022/main?labpath=notebooks)

If you are having issues with that (ex. it is taking a long time), try using the following link:
```
https://hub.aws-uswest2-binder.pangeo.io/user/{your_github_username}/lab
```
Where you replace `{your_github_username}` with your github username (ex. `mgrover1`)

#### General Binder Advice

The simplest way to interact with a Jupyter Notebook is through
[Binder](https://mybinder.org/), which enables the execution of a
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
Jupyter](https://foundations.projectpythia.org/foundations/getting-started-jupyter.html).

### Running on Your Own Computer
If you are interested in running this material locally on your computer, you will need to follow this workflow:

1. Clone the `https://github.com/mgrover1/mscar-python-workshop-2022` repository:

   ```bash
    git clone https://github.com/mgrover1/mscar-python-workshop-2022.git
    ```  
1. Move into the `mscar-python-workshop-2022` directory
    ```bash
    cd mscar-python-workshop-2022
    ```  
1. Create and activate your conda environment from the `environment.yml` file
    ```bash
    conda env create -f environment.yml
    conda activate mscar-python-tutorial-dev
    ```  
1.  Move into the `notebooks` directory and start up Jupyterlab
    ```bash
    cd notebooks/
    jupyter lab
    ```
