# Active learning for multimetallic catalyst design for higher alcohol synthesis (HAS)

This repository contains the code for the paper title Active learning streamlines development of high performance catalysts for higher alcohol synthesis.

- [Overview](#overview)
- [System Requirements](#system-requirements)
- [Installation Guide](#installation-guide)
- [Data preparation](#data-preparation)
- [Model training](#training)

# Overview

This repository contains the codes and dataset to train models for an active learning loop using the Gaussian process surrogate model with the Bayesian optimization.  
This repository contains the following:

* There are three jupyter notebooks, specific to three distinct phases of the research project.
* For each notebook, we provide the curated data in clean Excel sheets which are labelled corresponding to the phases.
* Necessary instructions to run the model and expected outcome are provided as comments in the notebook.

# System Requirements

## Hardware requirements
The code can run on any standard computer.

## Software requirements
The package has been tested on the following systems:
+ Windows 11 Pro for Workstations with 64-bit operating system, x64-based processor

### Python

A Python version of 3.7 or above is recommended. Most of the code is developed using standrad library packages including:

* Pandas 2.0.3 
* Numpy1.24.3 
* Scikit-learn 1.3.0
* Tensorflow 2.12.1
* GPflow 2.9.0
* Trieste  
* Shap 0.40.0

- # Installation guide

To use the package, we recommended to create a dedicated `conda` or environment, for example:

* conda create -n active-learning python=3.7
* conda activate active-learning

The codes can also be run on an exisiting environment provided the above listed packages are systemically installed using pip or conda commands.

- # Data preparation

We provide the clean and labelled curated data as Excel sheets  corresponding to the phases. Users do not have to do additioanl data-processing and can simply use the codes and by linking with the appropriate datasheet.

- # Model training

The workflow uses standard training process for implementing the Gaussian process and we provide detailed instructions for the same. The hyperparameters of the Gaussian process are optimized using inbuilt optimizer in GPflow. Implementing the Bayesian optimizer (BO) needs intermediate knowledge of Python. Though we provide instructions to run the BO specific to our datasets and case studies, we also refer to the tutorial found at (https://secondmind-labs.github.io/trieste/3.1.0/tutorials.html) for enhanced understanding. The expected outcome after the end of the BO campaign and its implication to this research project is explained in the notebooks.














