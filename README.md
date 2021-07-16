# Image-Recognition-using-transfer-learning-ML

# Transfer Learning for Image recognition
## A ML model for image recognition using transfer learning.

General info
The aim of this repository was to create a simple image recognition model using the weights of a pre-trained model as starting point for our model (pre-trained model weights were learned on ImageNet for this specific example but, any of the pre-trained Keras Applications Models can be used here). The weights from the pre-trained model are not trainable in this example (its layers are frozen with this purpose). This model is composed of a pre-trained set of layers (number of layers and model structure depend on the chosen base model) with an additional model on top of them, which is composed by six Dense layers. Five of these layers use a Relu function as their activation function and the last one uses a Softmax in order to assign probabilities to the model output. Please, note that the 5th layer of the vanilla Neural Network on top of the pre-trained model has been named as "extraction", in order to facilitate feature extraction from this model for any other task (e.g. Image captioning using seq2seq).

# Project structure
This repository contains only one file which must be executed in the following order:

Pre-trained model and New model on top (mainmodel.py)

## Libraries
The following Python libraries were used in this repository:

* Tensorflow Keras and TF Keras Preprocessing
* Os
