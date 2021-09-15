# COVID-19 Pandemic and Air-Quality
## Introduction
Nitrogen Dioxide (NO2), one of the major pollutants, results from vehicular, industrial, and
thermal power plant emissions. During the COVID-19 pandemic, a [nationwide lockdown](https://en.wikipedia.org/wiki/COVID-19_lockdown_in_India) was
imposed into four phases from March 25 - May 31, 2020; Phase-I (25/03/2020 - 14/04/2020),
Phase-II (15/04/2020 - 03/05/2020), Phase-III (04/05/2020 - 17/05/2020) and Phase-IV
(18/05/2020 – 31/05/2020). All major anthropogenic activities contributing to atmospheric
pollution (such as industries, vehicles, and other activities) were restricted during the lockdown.
The current report investigates the impact of the lockdown on tropospheric NO2 concentrations
before and during the different phases of lockdown through satellite obsevation and groundbased
(CPCB) measurement across India and two major cities Delhi and Bangalore. Sentinel-5P NRTI NO2:Near Real-Time Nitrogen Dioxide dataset has been used for the analysis and is directly imported from the [GEE Image Collection](https://developers.google.com/earth-engine/datasets/catalog/COPERNICUS_S5P_NRTI_L3_NO2#description). [GeeMap](https://geemap.org/), a Python package for interactive mapping with [Google Earth Engine](https://earthengine.google.com/) API is used for the analysis.


## Files 
### Input
- The input folder contains all the input files.
### Output
- The input folder contains all the input files.
### requiremet.txt
- The Requirement file contains all the packages required to run the project.
### Air Quality.ipynb
- It is a Jupyter Notebook document containing all programs.
### Report
- It is the analysis part of the Project.
## How to run this Project? 
- Create a virtual environment

```
conda create -n env python=3.8
```
- Activate the Environment and install all the required packages
 
```
conda activate env
pip install pandas
pip install matplotlib
pip install geemap
conda install geopandas
conda install mamba -c conda-forge
mamba install geemap xarray_leaflet -c conda-forge
conda install jupyter_contrib_nbextensions -c conda-forge
```
Required packages can also be installed using the Requirement.txt file
```
pip install requirement.txt

```
- Run Air Quality.ipynb file in Jupyter notebook
### Note:
- Please check all the input paths and the requirement carefully.

### Outputs 
- NO2 level(µmol/m^2) in 2019 and 2020

![2019](/output/India/PNG/2019.png) ![2020](/output/India/PNG/2020.png)

- No2 comparision in 2019 and 2020 during the lockdown
 
![2019_lockdown](/output/India/PNG/2019_lockDown.png) ![2020_lockdown](/output/India/PNG/2020_lockDown.png)

- NO2 level during the lockdown phases

![Pre lockdown](/output/India/PNG/PreLock-Down_IND.png) 

![phase-I](/output/India/PNG/Phase_I_IND.png)

![phase-II](/output/India/PNG/phase_II_IND.png) 

![phase-III](/output/India/PNG/Phase_III_IND.png)

![phase-IV](/output/India/PNG/phase_IV_IND.png)

## NO2 level(µmol/m^2) over Delhi

- Pre lockdown and Phase-I lockdown

![Pre lockdown_Delhi](/output/Delhi/PNG/pre-lockDown_Delhi.png) ![Phase_I_Delhi](/output/Delhi/PNG/phase_I_Delhi.png)

- Phase-II and Phase-III lockdown

![Phase_II_Delhi](/output/Delhi/PNG/Phase_II_Delhi.png)         ![Phase_III_Delhi](/output/Delhi/PNG/phase_III_Delhi.png)

- Phase IV lockdown

![Phase_IV_Delhi](/output/Delhi/PNG/Phase_IV_Delhi.png)

## NO2 level(µmol/m^2) over Bangalore

- Pre lockdown and Phase-I lockdown

![Pre lockdown_Bang](/output/Bang/PNG/Pre-lockDown_Bang.png) ![Phase_I_Bang](/output/Bang/PNG/phase_I_Bang.png)

- Phase-II and Phase-III lockdown

![Phase_II_Bang](/output/Bang/PNG/Phase_II_Bang.png)         ![Phase_III_Bang](/output/Bang/PNG/phase_III_Bang.png)

- Phase IV lockdown

![Phase_IV_Bang](/output/Bang/PNG/phase_IV_Bang.png)

## Time-Series analysis over Delhi

![Delhi](/output/Time-Series/Delhi.png)

## Time-Series analysis over Bangalore

![Bang](/output/Time-Series/Bang.png)

## Refrences

- [geemap](https://joss.theoj.org/papers/10.21105/joss.02305)

- [GEE](https://doi.org/10.1016/j.rse.2017.06.031)

- [Copernicus Sentinel-5P](https://doi.org/10.5270/S5P-s4ljg54)

