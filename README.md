# Deep Learning for Cryptocurrency Price Prediction
<div float="left">
  <img src="https://www.tensorflow.org/images/tf_logo_transp.png" height="120" >
  <img src="https://s3.amazonaws.com/keras.io/img/keras-logo-2018-large-1200.png" height="120">
</div>
<div float="right">

</div>

## 

### Introduction
This repo makes use of the state-of-art Deep Learning algorithm to predict the price of Bitcoin, which has the potential to generalize to other cryptocurrency. It leverages models such as CNN and RNN implemented by [Keras](https://github.com/keras-team/keras) running on top of [Tensorflow](https://github.com/tensorflow/tensorflow). You can find more detailed illustration in this [blog post](https://blog.goodaudience.com/predicting-cryptocurrency-price-with-tensorflow-and-keras-e1674b0dc58a).

### Getting Started
To run this repo, be sure to install the following environment and library:

1. Python 2.7
2. Tensorflow=1.2.0
3. Keras=2.1.1
4. Pandas=0.20.3
5. Numpy=1.13.3
6. h5py=2.7.0
7. sklearn=0.19.1

### File Illustration
#### There are currently three different models:
1. LSTM.py
2. GRU.py
3. CNN.py (1 dimensional CNN)

#### The validation result is plotted in:
1. Plot_LSTM.ipynb
2. Plot_GRU.ipynb
3. Plot_CNN.ipynb

#### Data is collected from [poloniex](https://poloniex.com) and parse to h5py file:
1. DataCollection.ipynb
2. PastSampler.ipynb

### Run
To run the prediction model, select one of the model. For instance, 
```
python CNN.py
```
To run iPython file, you need to run jupyter notebook
```
jupyter notebook
```
__Be sure to run DataCollection.ipynb and PastSampler.ipynb first to create database for training models.__
