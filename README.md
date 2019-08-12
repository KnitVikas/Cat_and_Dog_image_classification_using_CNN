# cnn_using_dogsAndcats

Cats And Dogs Image Classification
we are building this model with neural networks. Here i am using the keras to do classification. keras is the neural network library which work on top of the Tensorflow or we can say tf as the backend for this library.

DATA: we have downloaded our data from the kaggle website you can download it from here : https://www.kaggle.com/c/dogs-vs-cats/data

Here we use simple sequential neural networks which allow us to to use neural nets only layer by layers it does not allow you any complex neural nets such as RNN and LSTM. These neural networks are form simply layers by layes and each layers have their own weights. imput of one layers feeded to another. The sum of the product of current weights and input from previous layers form the activations to next layer.

finally in last layer we have flatten these hiddden layers and the last layer is the sigmoid layers which outputs as the Dog or Cat. SIGMOID is generally used for the classification purpose only.

The ADAM OPTIMIZER algorithm which is an extension to stochastic gradient descent.It is useful to give a global optimal solution So we have used it here for optimization.

ACTIVATION FUNCTION used is the he Rectified Linear Unit (ReLU) In a neural network,the activation function is responsible for transforming the imputssummed weighted input from the node into the activation of the node or output for that input.

To minimize the loss of the weights and activations we have used the binary_crossentrpy function here.A metric is function that is used to judge the performance of your model


Initialising the CNN:


Here i have added various layers. About these layers i discussed above . convolution function takes three arguments the first is about the number of output i. 32 . the filter used here is of size 3X3. the input size of the image is 64x64 pixel the rgb channel used is of size three. Hence the input size becomes as 64x64x3.

The maxpooling size is 2x2. i.e from ech matrix of image we wll filter the matrix according to feature with max occurance. the number of layers could be added according to the combination which gives you the best accuracy.


Data Augmentations

This is done so to increase the diversity of data so as to give more insights of the images to the machine algorithms. Here we use shearing, zooming the images and making the horizontal flip of images technique to train our neural nets.


Loading Data

Here i have loaded my data from my local file the data is freely available to kagggle site there are almost 25000 images of cates and dogs. out of 25000 images we can break it as 15000 for ur training and 10000 as our test datasets. i have used only 8000 images for train and 2000 for test purpose.

we will break our images as 64x64 pixels images. and batch_size is the number of images per epoch to be feed to our algo.


Training our data

Here we have fitted our data to the neural networks.Classifier is the instance of the sequential classifier which is the simplest neural network which form the layers of nearons. Here we include 100 images per epochs and the total epochs will be 55 validation data is nothing but our test set which consist of 2000 images in our case.
.
The accuracy we get is approx 84 percent which is good as we have taken small trainig example and the simple neural networks.

RUN:

Notebook

Requirement:

Anaconda Distribution.
Python3.6
