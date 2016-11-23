# Recognise Streetview Digits

My final project for the [Udacity machine learning engineer nanodegree course](https://www.udacity.com/course/machine-learning-engineer-nanodegree--nd009) was to build a deep convolutional neural network in TensorFlow to recognise digits from the streetview house number dataset.

This might be interesting for you if you want an example of how to build a deep CNN in tensorflow that is:
- **integrated into TensorBoard**, logging all interesting variables and letting you view the graph
- **parameterised**, building the network based on a set of hyperparameters that specify the depth, convolution sizes, learning rates, regularisation approach, etc
- **inspectable**, returning not just the predictions but also the weights and the logits of the test set to explore what's happening

The code for this project is contained entirely in five iPython notebooks:

1. Data load and exploration.ipynb
1. Data preprocessing.ipynb
1. Implementation.ipynb
1. Performance and visualisation.ipynb
1. Create new test set.ipynb

The Python version used was 2.7.6.

All required import modules are shown at the top of each notebook. The main modules are 
- tensorflow
- numpy, pandas, scipy, random
- os, sys, tarfile, six.moves
- matplotlib, seaborn
- timeit, time

Input files for training and testing can be dowloaded from http://ufldl.stanford.edu/housenumbers/

Test images taken with my camera are in the test_photos folder in the zip file containing the project submission.
