# Simulation-Self-Driving-Car

## Overview
Self-driving car model using advanced technologies and machine learning techniques. The project, required a comprehensive understanding of neural networks, and computer vision. I successfully implemented a Convolutional Neural Network (CNN) architecture for both training and testing modes, leveraging libraries such as numpy, matplotlib, TensorFlow, and Keras. The architecture employed two inputs, steering angle, and a set of cameras, demonstrating my proficiency in integrating diverse technologies. Additionally, the project involved rigorous testing methodologies, including unit testing, integration testing, and user acceptance testing, ensuring the reliability and functionality of the self-driving car model. This endeavor not only honed my technical skills but also fostered my problem-solving abilities in the realm of autonomous systems."

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
-Open anaconda powershell
-Navigate to source folder
-Open Udacity Simulator in Autonomous mode

Activate environment and Run model
```python
conda activate car-behavioral-cloning
python drive.py model.h5
```
