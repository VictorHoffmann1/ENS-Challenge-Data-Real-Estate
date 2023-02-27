# ENS-Challenge-Data-Real-Estate
This challenge organized by ENS Ulm and Collège de France was about predicting real estate prices with tabular data and images.
One of the main the difficulties of this challenge was that we had two types of data: tabular data and images. Moreover, each real estate good contained between 1 and 6 images, which all had different sizes. Therefore, a lot of efforts into data importation had to be put. Additionally, NaN values have been replaced by the median value of the variable if it was a numerical one or by the most common observation if the variable was categorical. Some variables that seemed useless or redundant for training have been removed and the categorical data has been target encoded.

When it comes to creating model, I decided to make a concatenation of a multilayer perceptron (MLP) for the tabular data and a convolutional neural network (CNN) for the images using Keras. 

You can find the code that I've written (jupyter notebook) in this repository. 
