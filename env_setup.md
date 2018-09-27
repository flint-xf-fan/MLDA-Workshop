# Python Environment (local, CPU-only) Setup Guide

## Download and install Anaconda
Choose Python 3.6 version: https://www.anaconda.com/download/#macos

(for windows only) Install Git: https://git-scm.com/downloads

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
