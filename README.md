## Description

Kaggle Digit Recognizer Competition: Learn computer vision fundamentals with the famous MNIST data. (https://www.kaggle.com/c/digit-recognizer) 

MNIST data is released in 1999, this classic dataset of handwritten images has served as the basis for benchmarking classification algorithms. It is a reliable resource for researchers and learners.

The dataset consists of pair, “handwritten digit image” and “label”. Digit ranges from 0 to 9, meaning 10 patterns in total.
handwritten digit image: This is gray-scale image with size 28 x 28 pixel (784 columns).
label : This is actual digit number this handwritten digit image represents (1 column). It is either  0 to 9.

The goal is to correctly identify digits from a dataset of tens of thousands of handwritten images. The training data includes 42000 digits. The training data are used to train the model and to predict 28000 digits in the test data. 

To solve the problem, several models are applied and compared, including KNN, Random Forest, CNN, CNN with data augmentation and ResNet. CNN with data augmentation performs the best among all of them, with the training accuracy of 99.81% and validation accuracy of 99.64%. 

_______________________________________________________________________________

## Overview

#### Feature Engineering: 
Performing a grayscale normalization to reduce effect of illumination differences and help the models converge faster.
In CNN and ResNet, they are reshaped to 28*28

#### Architecture (In CNN & ResNet): 
convolution layer | pooling | batch normalization | dense layer | dropout 

#### Hyperparameters Tuning (In RF, KNN, CNN & ResNet):
Grid search is used

#### Confusion Matrix:
Used to evaluate multi-classification results

#### Results Testing:
Prediction results of 28000 digits are tested in Kaggle

