# DL_Project2
Image Classification of keras dataset CIFAR 10 using CNN Model

This repository contains ipython notebook.This notebook has the code to build a CNN model which classifies keras CIFAR 10 dataset.There are 10 classes namely 'airplane','automobile','bird','cat','deer','dog','frog','horse','ship','truck'. Using image preprocessing, images are taken in (32*32) size. And it is rescaled to 1/255 for using it into the model.

Sequential is imported from keras. 2 Conv2D layers are added with first with 32 filters and second with filters of (3*3) size and relu as activation function. Each of them are followed by a MaxPool2D layer with pool size of (2*2) and strides 2. Half of the nodes are dropped using Dropout.  Flatten is used to flatten the data. Then, 2 dense layers(fully connected neural networks) are added. First with 128 units and relu as activation function. And, Second with 10 units and softmax as activation function because there is classification among 10 classes.


Model is created and fit with X_train and Y_train with 10 no. of iteration. Now,learning curve is plotted.
Result: 'loss':0.7440102100372314  'sparse_categorical_accuracy':  0.7369800209999084' val_loss': 0.7899489998817444],'val_sparse_categorical_accuracy': 0.7281000018119812
