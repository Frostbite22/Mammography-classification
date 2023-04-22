# Mammography images classification using Pytorch
This is a deep learning project for mammography images classification using Pytorch. We have used the Digital Dataset for Screening mammography, containing 11,219 images, devided between benign, normal and malignant.

## Data Preprocessing 
First we had to seperate our data into three main folders, train, validation and test for each class ( benign, normal, malignant). We gave training almost 70% of the data while dividing the rest between test and validation. <br>
No big transformations were applied to the images other than normalizing the data to train faster.

## Model
We have used a convolutional neural network model and stacking ReLU activations between convolutions blocks. We finally trained the model with a dropout to avoid overfitting for 20 epochs. 

## Optimizer and Loss Function 
Adam Optimizer and CrossEntropyLoss functions were used with the standard parameters for the optimizer ( learning rate = 0.001 )

## Results 
We can achieve 93% of the training set and 82% on the test set using 20 epochs of training
