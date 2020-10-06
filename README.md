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

The library tf-js vis is used for visualization of the training process  

Because we training in the browser we use Spread Sheet to load the dataset, we stick all the training images together into a single image.  

We have 60,000 training images and 10,000 testing images

You can draw digits on the black rectangle to be classified. After drawing a digit, and pressing the "classify" button, the code will alert the predicted digit.

In the mnist.html:  

Load the javascript libraries tensorflow.js and tfjs-vis.js  
A canvas 280x280 in which we are going to draw a something  
Conver canvas to an image  
Two buttons one to classify the drawing and one to cleas the canvas  
Two javascript scripts as imported: data.js and the script.js  
The data.js file contains the mnist class which downloads the sprites, slices it up, download the labels and give you batches that you can load into the classfier    
The script.js file contains the handling of the canvas, it has the infrence and has the training  

To run this project you need a web server, the chrome server is used : https://www.chromebeat.com/ 



