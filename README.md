## Using a deep convolutional neural network to recognise numbers in images

My final project for the [Udacity machine learning engineer nanodegree course](https://www.udacity.com/course/machine-learning-engineer-nanodegree--nd009) was to build a deep convolutional neural network in TensorFlow to recognise digits from the [streetview house number dataset](http://ufldl.stanford.edu/housenumbers/).

Why might this be interesting? If you're getting in to deep CNNs and want to see an example in tensorflow that is:
- **integrated into TensorBoard**, logging all interesting variables and letting you view the graph
- **parameterised**, building the network dynamically for each run based on a list of hyperparameters
- **inspectable**, returning not just the predictions but also weights and test logits to see what's going on
- **reasonably good on a CPU**, with 92% accuracy achieved in 9 hours training time.

The code for this project consists of five iPython notebooks:

1. [Data load and exploration](../master/1%20Data%20load%20and%20exploration.ipynb)
1. [Data preprocessing](../master/2%20Data%20preprocessing.ipynb)
1. [Implementation](../master/3%20Implementation.ipynb)
1. [Performance and visualisation](../master/4%20Performance%20and%20visualisation.ipynb)
1. [Create new test set](../master/5%20Create%20new%20test%20set.ipynb)

The solution was inspired by Ian J. Goodfellow, Yaroslav Bulatov, Julian Ibarz, Sacha Arnoud, Vinay Shet's paper [Multi-digit Number Recognition from Street View Imagery using Deep Convolutional Neural Networks](http://static.googleusercontent.com/media/research.google.com/en//pubs/archive/42241.pdf).

The implementation module builds a graph that looks something like this (depending on the layers you specify):
![alt text](../master/Images/Tensorboard_graph.png)

With convolutional layers that look like this:
![alt text](../master/Images/Tensorboard_graph_zoom.png)

Generating learning curves that look like this:
![alt text](../master/Images/Learning_curves.png)

Producing results that look like this:
![alt text](../master/Images/results.png)

The Python version used was 2.7.6. The main modules used were: 
- tensorflow
- numpy, pandas, scipy, random
- os, sys, tarfile, six.moves
- matplotlib, seaborn
- timeit, time
