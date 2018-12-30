# Repo for MLDA Workshops
* sponsored by MLDA@EEE
* This repo may refer to some online materials/MOOCs and it is for educational purpose only. Pls contact Xiaofeng(fxf1996@gmail.com) if any unapproriated use found.


# Python Environment (local, CPU-only) Setup Guide

## Download and install Anaconda
Choose Python 3.x version: https://www.anaconda.com/download/#macos

## Env Setup
### 1. Create Environment
Open a terminal(for Mac) / Anaconda Prompt(for Windows),  type command

`$ conda create -n DIP python=3.6`

Then
* for Windows, type: `$ conda activate DIP`
* for mac/linux, type: `$ source activate DIP`

### 2. Install packages
Type command:
`$ conda install pandas numpy scikit-learn matplotlib tensorflow keras jupyterlab ipykernel`

`$ pip install pillow opencv-python`

### 3. Validate your installation
Type command:
`$ jupyter lab` to start the interactive notebook for your experiments. By default, a service will be running at http://localhost:8888/. You can access it using any browser.

Then create a notebook, run the following code:
```
import keras
import matplotlib
import numpy as np
import pandas as pd
import tensorflow as tf
```

You should see no error.

# Setup on your GPU server
You are given an account to access one of our GPU stations (Tesla V100 or GTX 1080 Ti) at EEE AI Lab. 
## To connect to the server
`$ ssh your_username@IP_ADDRESS`

## Install Anaconda
Run following commands:
```
$ cd ~
$ wget https://repo.anaconda.com/archive/Anaconda3-5.3.0-Linux-x86_64.sh
$ bash Anaconda3-5.3.0-Linux-x86_64.sh
```
Then make response accordingly.
