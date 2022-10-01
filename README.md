This code is for a model of a K Nearest Neighbors algorithm.

Preprocess.py reads the data file, then orients the data in a way that allows the KNN model to work. The functions: get_data_MNIST() and get_data_CIFAR() takes in the data folder path, then given a string, returns the images for the training or testing set. get_specific_class() returns a specific number of examples for a given class. get_subset() returns a specific number of examples of each class.


KNN_Model.py is the file that implements the K-Nearest Neighbors algorithm. It is a class that is initiallized with a value for k (k==9 for this assignment), and a list of the class names. fit() is used to train the model, which lays out the data points and the labels. get_class_counts() returns a list containing the number of occurrences of the classes among the neighbors (class_counts) and a list of the indicies of the nearest examples. predict() returns a prediction for a new data point and get prediction_array() returns an array of predictions for an array of data points.


HW1_MNIST.ipynb is the notebook for implementing the KNN model on the mnist dataset. The model performed with an accuracy of 0.9148.

HW1_CIFAR.ipynb is the notebook for implementing the KNN model on the CIFAR dataset. The model performed with an accuracy of 0.232. This notebook also included the use of the ResNet model. This, performed with an accuracy of 0.612
