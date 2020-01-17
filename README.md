# Modak_Image_Classification
Implementing convolutional neural network using keras library to classify Modak(Dessert) images

# Collection of Data

First of all collection of the data takes place. I use Google Image downloader to download the images of modak which is 425.I wanted to make images of constant size
All images of modak is resolution of 500*500.I keep 345 images for the training and rest 80 for the testing. I take other Indian famous dessert
as a non_modak like barfi,laddu,gajar ka halwa,jalebi,gulab jamun,rossogulla,aflatoon dessert etc. And I also add MOMOS in non_modak since it looks same.

# Augmentation of Data

Using keras's ImageDataGenerator i augmented rescale, shear_range=0.2, zoom_range=0.2, horizontal_flip=True in the training data.
and i did only rescaling in the testing data.

# Training the model

using keras implement two convolutional neural network followed by maxpool followed by flatten and dense layer. I use Binary_crossentropy as a
loss function, and AdamOptimizer as optimizer.Then train the model with 50 epochs.

# 1:- In the modak_calssifier1 notebook i added momos images in the non_modak class then after 50 epochs i get 40% highest accuracy
# 2:- After Excluding MOMOS from non_modak class in the modak_calssifier notebook the accuracy jumped almost double after 50 epochs which is 83% highest
        
