# Neural_tutorial
## What am I doing here? 
This is rough around the edges Artificial Neural Network (ANN) tutorial I developed to get started with ANNs in python. I am using Jupyter notebooks and Python 3. The ANN structure for the NN_tutorial is primarily based on this Medium post https://towardsdatascience.com/how-to-build-your-own-neural-network-from-scratch-in-python-68998a08e4f6 and inputs for NN_tutorial are based on this towards data science post https://towardsdatascience.com/artificial-neural-networks-for-total-beginners-d8cd07abaae4
 
# NN_tutorial: 
First (using above posts) I build a ANN from scrath in python using a simple 1 layer set-up - one hidden layer with four nodes and one output layer. Both layers use a sigmoid activation function. I wanted to get an idea of how forward and backpropogation works in a simple code. I also added a learning rate and may add a bias term. 

I go through a toy example using synthetic (made-up) soil moisture and soil grain size data to predict (made-up) CO<sub>2</sub> flux. I look at how predictions change based on the properties of the training data set. I create a cartoon/toy example that shows if your training data do not adequetaly span the full range of values, your model will not be able to "learn" how to make accurate predictions under "real world" conditions. This is a cartoon example but helps to clarify the basics of an ANN.

# Keras_simple:
I then build that same model using Keras which can handle all the optimization parameters/hyperparameters. A bit more black box but also quicker and easier.

# Predictor_processing:
This is a set of scripts to help me load in predictor and target data. Just a testing ground where I make some plots and investigate variable dimensions, etc...

# NN_sandbox: 
Next I train an ANN on inverse fluxes of net ecosystem exchange of CO2 over North America (from here https://iopscience.iop.org/article/10.1088/1748-9326/aad505). The goal here is to use reanalysis data to build an ANN to estimate net carbon fluxes using regional top-down estimates as a target. While ANNs have been used to estimate carbon fluxes using various fine scale flux data (e.g., FLUXCOM http://www.fluxcom.org/) and larger scale datasets (e.g., WECANN https://bg.copernicus.org/articles/14/4101/2017/), to date, no regional inverse fluxes have been used as target datasets for ANN model development. The efforts here hope to capture integrated processes inferred from the relatively dense atmospheric CO2 observation network over North America. While this ANN will not be able to capture more detailed processes it may offer insights into the drivers of emergent regional scale processes driving net CO2 fluxes, again over North America but possibly relevant to other Northern Hemisphere ecosystems.
