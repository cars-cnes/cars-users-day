# TP: Getting Started with CNES Open-Source 3D Tools in Python

Welcome to this tutorial on using open-source software developed by CNES for 3D reconstruction. This TP was created for the release of version 1.0 of CARS.

## Software Used

### CARS (Required)
- **CARS** is the software for producing Digital Surface Models (DSM) from pairs of satellite images. It generates both rasters (2.5D representation) and point clouds.

### Optional Software
- **Bulldozer**: Removes above-ground elements (trees, buildings, etc.) from DSMs to produce Digital Terrain Models (DTM).
- **SLURP**: Allows the production of land cover masks particularly useful for CARS, such as water masks to avoid unnecessary calculations on water areas.
- **xDEM**: Software for analyzing the 3D models produced by CARS and Bulldozer. Useful for comparing the models with reference data such as LiDAR HD.

## Study Areas
The tutorial will focus on two areas around Toulouse:
- **ROI_INDUS**: An industrial area 
- **ROI_STADIUM**: The area around the Stadium, located on an island surrounded by the Garonne

## Prerequisites
- A Google account to use Google Colab
- A stable internet connection

## Installation and Usage

### On Google Colab

#### Step 1: Open the Notebook on Google Colab
1. Go to [Google Colab](https://colab.research.google.com/)
2. Click on "New Notebook"
3. In the menu, go to "File" > "Open Notebook" and select the `.ipynb` file present in the GitHub repository

#### Step 2: Run the Google Colab
Run `tutorial.ipynb` and enjoy :)

### On the CNES jupyterhub

#### Step 1: Connect to the CNES jupyterhub 

1. Go to [the CNES JupyterHub](https://jupyterhub.cnes.fr/)
2. Use the correct username and password.
3. Choose the VRE

#### Step 2: Get the repo Github 

1. Open a terminal
2. `ml git`
3. `git glone https://github.com/cars-cnes/cars-users-day.git`

#### Step 3: Create your kernel

1. Open a terminal
2. `python -m env venv`
3. `source activate venv/bin/activate`
4. `pip install cars==1.2.0rc2`
5. `pip install slurp_masks-0.1-cp312-cp312-linux_x86_64.whl`
6. `pip install xdem[opt]`
7. `pip install ipykernel`
8. `python -m ipykernel ipykernel install --user --name=tuto_CNES --display-name="tuto CNES"`

#### Step 4: Run the notebook

1. Open the notebook `tutorial.ipynb`
2. Run it and enjoy :) 

