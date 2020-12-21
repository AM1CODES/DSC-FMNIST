# DSC-FMNIST
Repository for Second round interview for DSC Technical Team VIT-B

# Data
We have 70,000 images of size (28x28). This data set acts as a new replacement or alternative for the original MNIST data set and this too has 10 classes like the original MNIST data. <br>
Link to the data - https://www.kaggle.com/zalando-research/fashionmnist

# Our Goal
We had to use the data provided to us and create a multi-class classification ML or DL model.

# My approach
1) Started off by importing our data. We had 2 sets of data . A training set and a testing set. Both of these were available in the CSV format. <br>
2) After importing i looked at the columns of the data. We had values uptil 784 pixels(28x28) along with a labels column. <br>
3) To be able to train a CNN model we need to use keras, so we had to include one more dimension to our 28x28 data cause keras works with 3-D matrices. So after creating different training and testing sets, i normalized our data by dividing the training and testing set by 255 so that the value ranges between 0 and 1. Normalizaton helps our model perform better. We also reshaped it and converted the images in grayscale to feed as the input to train the model. We also performed one hot encoding for our labels as we have categorical data. <br>
4) We then split our data and created our custom CNN model along with specifying the batch size and number of epochs for which we will train our model. <br>
5) We performed some data augmentation to help the model train better and prevent overfitting. It basically creates more variations in the data that we feed the model to train on. <br>
6) We trained our model for the specified number of epochs and were able to get some results. <br>

# Results
We were able to achieve an accuracy of 89% on training as well as testing set but these aren't great results and the model can be enhanced  a lot by maybe increasing the number of layers we have or by increasing the number of filters that we have and so on.
