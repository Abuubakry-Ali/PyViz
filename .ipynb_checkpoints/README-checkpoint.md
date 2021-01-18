# Toronto Real Estate Market Analysis for 2001 - 2016

![Toronto at night](images/toronto.jpg)

The purpose of this project was to create a dashboard that a real estate investment company can provide customers interested in the Toronto market. The dashboard's goal is to provide charts, maps, and interactive visualizations that help customers explore the data and determine if they want to invest in rental properties in Toronto.
In the end, the following tools were presented: 


- a notebook of rental analysis
- a dashboard of interactive visualizations to explore the market data


The data in this dashboard was retrieved from the following websites:

Toronto Open Data
Census Profile, 2016 Census - Toronto Metropolitan Area, Ontario and Canada

## Getting Started
####To open dashboard 
 * Download the folder 
 * using command prompt navigate to folder 
 * Run command 
    * panel serve dashboard.ipynb --log-level debug --showThese instructions will get you a copy of the project up and running on your local machine for development and testing purposes. See deployment for notes on how to deploy the project on a live system.



## Usage

#### Step 1: Conda with PyViz

You will need to have your conda environment activated with PyViz installed. 

Example:
```
conda activate dev
```

#### Step 2: Export the Mapbox Token

For this solution, you will need to export the mapbox token.

In the keys.sh file, enter the following:

```shell
export mapbox="ENTER YOUR API KEY HERE"
```

Activate the keys file:
```shell
. ./keys.sh
```

#### Step 3: Serve the Dashboard

```shell
panel serve --show dashboard.ipynb
```

---

## Installation Notes

Note: Skip these steps if you have already setup your environment using the PyViz installation guide.

Follow the below steps to install and set up PyViz in your Python environment. These steps should be completed outside of class.

1. Download the PyViz dependencies **nodejs** and **npm** (included in nodejs).

```shell
conda install -c conda-forge nodejs
```

2. Use the `conda install` command to install the following packages: hvPlot, Plotly Express, and Panel.

```shell
conda install -c pyviz hvplot
conda install -c plotly plotly
conda install -c pyviz panel
```

3. PyViz installation also requires installation of Jupyter Lab extensions. These extensions are used to render PyViz plots in Jupyter Lab. Execute the below commands to install the necessary Jupyter Lab extensions for PyViz and Plotly Express.

```shell
jupyter labextension install @pyviz/jupyterlab_pyviz
jupyter labextension install @jupyterlab/plotly-extension
```

4. Use the `conda list | grep pyviz` function to confirm installation of all PyViz packages. Look for `hvplot`, `panel`, and `pyviz_comms`.

```shell
conda list | grep pyviz
```

```
hvplot                    0.4.0                      py_0    pyviz
panel                     0.6.0                      py_0    pyviz
pyviz_comms               0.7.2                      py_0
```

5. Use the `conda list | grep plotly` function to confirm all Plotly packages are available. Confirm `plotly` and `plotly express` are listed.

```shell
conda list | grep plotly
```

```
plotly                    4.0.0                      py_0
plotly_express            0.4.0                      py_0  plotly
```

---



## Results
After analysis of data, a dashboard was created for customer use. Sample images can be seen below:


