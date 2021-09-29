<h1 style="text-align: center;  font-weigth: bold; margin-top: 20px;">
  Visual exploratory data analysis with python and pydeck
</h1>
<h2 style="text-align: center; margin-bottom: 10px;">
  Lorenzo Perozzi
</h2>
<p style="text-align: center; margin-bottom: 20px;">
   <a href="https://www.unige.ch/ge-rgba/welcome/">GE-RGBA Group, Departement of Earth Science, University of Geneva</a>
</p>
<div style="text-align: left;margin-bottom: 20px;">
    <img src="src/logo.png" style="height: 70px">
</div>


 
## About

During this tutorial, it will be shown how to use python to process and visualize a dataset consisting of geothermal probes availability in the Canton of Geneva. This dataset can be obtained (open access) through the <a href="https://ge.ch/sitg/fiche/6867 ">SITG</a> (Système d’Information du Territoire à Genève). We will cover these aspects:

- Load the geothermal probes dataset.
- Convert CRS coordinate system with **pyproj**
- Extract depth information form attributes
- Visualising the results with **pydeck**

|         | Info |
|--------:|:-----|
| When | Friday, October 1st • 12:30 - 13:00  |
| Live stream | Registration mandatory - [Under this link](https://formulaire.unige.ch/outils/limesurvey3/index.php/268393?lang=fr) |
| conda environment  | `DST-geothermal-visual` |
| Documentation | [deck.gl](https://deck.gl/) |



## Setup

If you want to follow along the tutorial, make sure you've done these steps **before the tutorial begin**:

### Step 1

**Install a Python distribution:**

In this tutorial we will be using the [Anaconda](https://www.anaconda.com/)
Python distribution along with the `conda` package manager. If you already have
Anaconda or Miniconda installed, you can skip this step.

If not, please follow the instructions for getting Anaconda up and running in
your system: https://docs.anaconda.com/anaconda/install/

### Step 2

**Create the `DST-geothermal-visual` conda environment:**

1. Download the `environment.yml` file from
   [here](https://github.com/geoenergy/DST1_pydeck_visual/blob/master/environment.yml)
   (right-click and select "Save page as" or similar)
1. Make sure that the file is called `environment.yml`. Windows sometimes adds a
   `.txt` to the end, which you should remove.
1. Open a terminal (*Anaconda Prompt* if you are running Windows). The
   following steps should be done in the terminal.
1. Navigate to the folder that has the downloaded environment file
   (if you don't know how to do this, take a moment to read [the Software
   Carpentry lesson on the Unix shell](http://swcarpentry.github.io/shell-novice/)).
1. Create the conda environment by running `conda env create --file environment.yml`
   (this will download and install all of the packages used in the tutorial).
1. **Windows users:** Make sure you set a default browser that is **not Internet Explorer**.
1. Activate the conda environment: `conda activate DST-geothermal-visual`
1. Create a new kernel for this environment environment: `ipython kernel install --user --name=DST-geothermal-visual`
1. Start the JupyterLab server: `jupyter lab`
1. Jupyter should open in your default web browser. We'll start from here in the
   tutorial. 
   
   
<div style="text-align: left; margin-bottom: 100px;">

 </div>