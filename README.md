# FaceRecognitionChallenge
Machine learning - face recognition challenge


Introduction
Challenge Large Scale Machine Learning
Authors:
Pavlo Mozharovskyi (pavlo.mozharovskyi@telecom-paristech.fr), Umut Şimşekli (umut.simsekli@telecom-paristech.fr)
Fusion of algorithms for face recognition

The increasingly ubiquitous presence of biometric solutions and face recognition in particular in everyday life requires their adaptation for practical scenario. In the presence of several possible solutions, and if global decisions are to be made, each such single solution can be far less efficient than tailoring them to the complexity of an image.

In this challenge, the goal is to build a fusion of algorithms in order to construct the best suited solution for comparison of a pair of images. This fusion will be driven by qualities computed on each image.

Comparing of two images is done in two steps. 1st, a vector of features is computed for each image. 2nd, a simple function produces a vector of scores for a pair of images. The goal is to create a function that will compare a pair of images based on the information mentioned above, and decide whether two images belong to the same person.

You are provided a label set of training data and a test set without labels. You should submit a .csv file with labels for each entry of this test set.
The properties of the dataset:
Training data:

The training set consist of two files, xtrain_challenge.csv and xtest_challenge.csv.

File xtrain_challenge.csv contains one observation per row which contains following entries based on a pair of images, A and B say:

    columns 1-14 - 14 qualities on image A;
    columns 15-28 - 14 qualities on image B;
    columns 29-36 - 8 matching scores between A and B.

File ytrain_challenge.csv contains one line with each entry corresponding to one observation in xtrain_challenge.csv, maintaining the order, and has '1' if a pair of images belong to the same person and '0' otherwise.

There are in total 3.196.465 training observations.
Test data:

File xtest_challenge.csv has the same structure as file xtrain_challenge.csv.

There are in total 1.598.219 test observations.
The performance criterion¶

The performance criterion is the prediction accuracy on the test set, which is a value between 0 and 1, the higher the better.


