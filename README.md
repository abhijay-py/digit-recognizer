# digit-recognizer
 
## A model to recognize digits 0 through 9 from images.

The MNIST dataset was retrieved from Kaggle for this project and the model was evaluated on Kaggle as well.
This data was reshaped from a list of the greyscale values for each pixel from pixel 0 to pixel 783, to a 28x28 matrix representing the original form of the picture. The Keras package was used to create the following model.

Then, a convolutional neural network was used to train this model with the following parameters:

- Layer 1: Convolution Layer, 64 nodes, kernel size of 4, with a ReLU activation function.

- Layer 2: Convolution Layer, 64 nodes, kernel size of 5, with a ReLU activation function.

- Layer 3: Flattening Layer.

- Layer 4: Output Layer, 10 nodes, each corresponding with a digit 0-9, with a softmax activation function.

This model was trained with a 0.1 validation split across 3 epochs using the Adam optimizer and categorical cross-entropy loss metric. This model was then stored in the digit-recognition-kernel-45.keras file.

This model scored a ***97.182% accuracy*** on the test set.

