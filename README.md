# Acoustic Project

## Overview

This repository is composed of two notebooks :
- tutorial-s3.ipynb (to load the files)
- acoustic.ipynb (the primary code)



Below, we provide a brief summary of the project, the libraries used, and an outline of the content within the notebook.
## Libraries Used

- numpy
- matplotlib
- pandas
- scipy
- scikit-learn
- tensorflow_hub
- keras



## Content of acoustic.ipynb

### 1. Initialization

- Set up datasets and parameters for consistency in model training.

### 2. Room Impulse Response (RIR)

- Explanation of RIR and loading RIR data from files.

### 3. Localizations

- Loading localization data from files.

### 4. Result Interpretation

- Functions for calculating mean distance between predicted and expected coordinates.

### 5. k-Nearest Neighbors and Linear Regression Models

- Introduction to RMS (Root Mean Square) and its use in model input preparation.
- Implementation of Linear Regression and k-Nearest Neighbors models.

### 6. Truncating the Inputs

- Testing the models with truncated input samples to observe the impact on performance.

### 7. VGGish

- Introduction to VGGish model for audio feature extraction.
- Loading and implementation of single channel VGGish using TensorFlow Hub.



## Content of tutorial-s3.ipynb
This is the architecture once the files are loaded

data/  
|-- LivingRoom_preprocessed_hack/  
|   |-- Empty/  
|   |-- deconvolved.npy  
|-- Human1/  
|   |-- centroid.npy  
|   |-- deconvoled_trim.npy  
|   |-- skeletons.npy  
|-- Human2/  
|   |-- centroid.npy  
|   |-- deconvolved_trim.npy  
|   |-- skeletons.npy

