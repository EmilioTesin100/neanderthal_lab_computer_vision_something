# neanderthal_lab_computer_vision_something
project for making use of CamHD data through computer vision

# Overview

This repo is in the making, but we hope to make a project for:
- Training and evaluation of specific hydrothermal vent structures of interest
- Training and evaluation of species-level classifiers for specific data sets
- Miscellaneous useful tools for examining data produced through our identifications

#### The Problem

To quantify the change in flocculent material in the water column above the ashes vent we must look at the same scene over time. However, the camera system is not consistent in it the where it looks at specific intervals. individual frame checking by a scientist is a laborious task that makes this study much more difficult. 

This project aims to use HD video frame data collected from the CAMHD in the OOI network to train a deep object recognition algorithm. With a learned model, its task will then be used to make predictions on non-annotated data. Predictions with high enough confidences will be retained as per the users discretion.

### Workflow at a glance:

1.) Parsing/cleaning existing annotation data  
2.) Extracting and organizing training data   
3.) Preprocessing and augmenting training data    
4.) Train object recognition/image classification network   
5.) Apply trained model to new data, take *good* predictions and add to training data   
