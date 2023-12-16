# Simulation-Self-Driving-Car

## Overview

## Dependencies
Install [anaconda](https://www.continuum.io/downloads) or [miniconda](https://conda.io/miniconda.html) to use the environment setting.

```python
# Use TensorFlow without GPU
conda env create -f environments.yml 

# Use TensorFlow with GPU
conda env create -f environment-gpu.yml
```
Or one can manually install the required libraries (see the contents of the environemnt*.yml files) using pip.

Additionally,
```python
pip install python-socketio==4.6.1
```

Finally install,
[Udacity self-driving simulator](https://github.com/udacity/self-driving-car-sim)

## Working
### To train the model
One needs the data folder which contains the training images.

```python
python model.py
```

This will generate a file `model-<epoch>.h5` whenever the performance in the epoch is better than the previous best.  For example, the first epoch will generate a file called `model-000.h5`.


### Run the model
Open anaconda powershell
Navigate to source folder
Open Udacity Simulator in Autonomous mode

Activate environment and run model
```python
conda activate car-behavioral-cloning
python drive.py model.h5
```
