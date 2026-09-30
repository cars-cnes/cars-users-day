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
- A Google account to use Google Colab or a CNES account
- A stable internet connection

## Installation and Usage

### On Onyxia

#### Step 1: Connexion
1. Go to [Onyxia](https://datalab.sspcloud.fr/)
2. Authenticate yourself or create an account if you don't already have one

#### Step 2: Use
1. Launch a `Jupyter-python` instance
2. Open a terminal and run `git clone https://github.com/cars-cnes/cars-users-day.git`
3. Go to `cars-users-day` folder and open the file `tutorial.ipynb` in a jupyter notebook

#### Step 3: Run the notebook

1. Open the notebook `tutorial.ipynb`
2. Run it and enjoy :) 

### On Google Colab

#### Step 1: Connexion
1. Go to [Google Colab](https://colab.research.google.com/)
2. Authenticate yourself to Google Colab

#### Step 2: Use
Download the file locally 
1. Click on "New Notebook"
2. Download this file on your computer: https://github.com/cars-cnes/cars-users-day/blob/main/tutorial.ipynb
3. In the menu, go to "File" > "Open Notebook" and select the `.ipynb` file present in your computer
Open the file from Github
1. Click on "Upload Notebook"
2. Select Github and add the following link: https://github.com/cars-cnes/cars-users-day/blob/main/tutorial.ipynb

#### Step 3: Run the Google Colab
Run `tutorial.ipynb` and enjoy :)

### On the CNES jupyterhub

#### Step 1: Connect to the CNES jupyterhub 

1. Go to [the CNES JupyterHub](https://jupyterhub.cnes.fr/)
2. Use the correct username and password.
3. Choose the VRE

#### Step 2: Get the repo Github 

1. Open a terminal
2. `ml git`
3. `git clone https://github.com/cars-cnes/cars-users-day.git`

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

