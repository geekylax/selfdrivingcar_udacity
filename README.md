# How_to_simulate_a_self_driving_car
This is the code for "How to Simulate a Self-Driving Car" by Siraj Raval on Youtube

And this model is an experiment that i gained from the youtube tutorial  and im trying to improvize this architecture in differnt scenarios

<img src="images/unity.gif" alt="Self-Driving Car" width="800px">
<!-- 
[![car]({{ site.url }}/images/unity.gif))]({{ site.url }}/images/unity.gif)) -->

## ToDo 

1. Check this repo and implement own Simulated car in unity [NFS](https://github.com/anubhavshrimal/Simulated_Self_Driving_Car) 
2. Check this model with weights 
3. Using CNNN with Backpropogation and check the performance 
4. Implenet RNN with different scenarios
5. improvize this model

## Overview

This is the code for [this](https://youtu.be/EaY5QiZwSP4) video on Youtube by Siraj Raval. We're going to use Udacity's [self driving car simulator](https://github.com/udacity/self-driving-car-sim) as a testbed for training an autonomous car. 

## Dependencies

You can install all dependencies by running one of the following commands

You need a [anaconda](https://www.continuum.io/downloads) or [miniconda](https://conda.io/miniconda.html) to use the environment setting.

```python
# Use TensorFlow without GPU
conda env create -f environments.yml 

# Use TensorFlow with GPU
conda env create -f environment-gpu.yml
```

Or you can manually install the required libraries (see the contents of the environemnt*.yml files) using pip.


## Usage


### Run the pretrained model

Start up [the Udacity self-driving simulator](https://github.com/udacity/self-driving-car-sim), choose a scene and press the Autonomous Mode button.  Then, run the model as follows:

```python
python drive.py model.h5
```

### To train the model

You'll need the data folder which contains the training images.

```python
python model.py
```""
""""""
This will generate a file `model-<epoch>.h5` whenever the performance in the epoch is better than the previous best.  For example, the first epoch will generate a file called `model-000.h5`.

## Credits

The credits for this code go to [naokishibuya](https://github.com/naokishibuya). I've merely created a wrapper to get people started.



