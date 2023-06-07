# CNN-on-CIFAR


# Description:

The CIFAR-10 data consists of 60,000 32x32 color images in 10 classes, with 6000 images per class. There are 50,000 training images and 10,000 test images in the official data. We have preserved the train/test split from the original dataset.  The provided files are:

train.7z - a folder containing the training images in png format
test.7z - a folder containing the test images in png format
trainLabels.csv - the training labels

To discourage certain forms of cheating (such as hand labeling) we have added 290,000 junk images in the test set. These images are ignored in the scoring. We have also made trivial modifications to the official 10,000 test images to prevent looking them up by file hash. These modifications should not appreciably affect the scoring. You should predict labels for all 300,000 images.

The label classes in the dataset are:

airplane 
automobile 
bird 
cat 
deer 
dog 
frog 
horse 
ship 
truck
The classes are completely mutually exclusive. There is no overlap between automobiles and trucks. "Automobile" includes sedans, SUVs, things of that sort. "Truck" includes only big trucks. Neither includes pickup trucks.


# Assignment:


Please visit this link to access the state-of-art DenseNet code for reference - DenseNet - cifar10 notebook link
You need to create a copy of this and "retrain" this model to achieve 90+ test accuracy.
You cannot use Dense Layers (also called fully connected layers), or DropOut.
You MUST use Image Augmentation Techniques.
You cannot use an already trained model as a beginning points, you have to initilize as your own
You cannot run the program for more than 300 Epochs, and it should be clear from your log, that you have only used 300 Epochs
You cannot use test images for training the model.
You cannot change the general architecture of DenseNet (which means you must use Dense Block, Transition and Output blocks as mentioned in the code)
You are free to change Convolution types (e.g. from 3x3 normal convolution to Depthwise Separable, etc)
You cannot have more than 1 Million parameters in total
You are free to move the code from Keras to Tensorflow, Pytorch, MXNET etc.
You can use any optimization algorithm you need.
You can checkpoint your model and retrain the model from that checkpoint so that no need of training the model from first if you lost at any epoch while training. You can directly load that model and Train from that epoch.


