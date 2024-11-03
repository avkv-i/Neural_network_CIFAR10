<h1>CIFAR-10 Neural Network</h1>

A neural network trained and tested using the CIFAR-10 dataset, composed of 60000 color images (3x32x32), each belonging to 10 classes. The training dataset consists of 50000 examples and a testing set composed of 10000 examples. 

First, a dataloader is created and then a neural network is created to classify the images. The architecture is composed of 3 intermediate blocks followed by an output block. Each intermediate block receives an image and has L number of convolutional layers working in sequence. The architecture is expanded upon and trained after inital implementation with various techniques. Kernel sizes, paddings, stride choices were used with batch normalisation and ReLu activation functions, inspired by ResNet architecture. The hyperparameters are the input channels (which are the subsequent output channels from the previous block), the output channels of each block, the dropout rate used, the learning rate and the beta parameters of the Adam optimiser used.ReLU activation functions were primarily used, the weights were initialised using Xavier initialisation which is a very popular technique. Regularisation techniques were also employed using various dropout layers, to reduce overfitting. 

*Note: The task required the use of the testing dataset as a validation dataset, to simplify the task.*
