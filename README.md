# Fashion-Mnist-using-Tensorflow.js
Convolutional Neural Networks for Image Classfication in the browser.   
Creating a ConvNet with Javascript
The architecture of the model consists of a sequence of layers:
conv2d : 2D convolutional layer with 28x28 monochrome images as input, kernel size 3x3, 8 filters and Relu activation function
maxPooling2d: pooling layer and it is a 2x2 pool
Conv2d : 2D convolutional layer with 28x28 monochrome images as input, kernel size 3x3, 16 filters and Relu activation function
maxPooling2d: pooling layer and it is a 2x2 pool
flatten: 28x28 images flattened out , so we have 784x1 images
dense: dense layer with 128 neurons and Relu activation function
dense: dense layer with 10 neurons and Softmax activation function
Fashion Mnist dataset show in a website using Tensorflow.js library. It runs on a Chrome Browser using Web Server an extension. 

The compile of the model consists of the following configurations:
Optimizer: adam
loss: categoricalCrossentropy
metric: accuracy

The training of the model consists of the following configurations:
epochs: 20

The library tf-js vis is used for visualization of the training process
