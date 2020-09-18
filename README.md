# CatsVSDogs-Classification

A fun project to differentiate dogs from cats.

## Pre-requisites:

- Python3
- pandas
- numpy
- NVIDIA® GPU card with CUDA® Compute Capability 3.5
- NVIDIA® GPU drivers —CUDA 10.0 requires 410.x or higher.
- CUDA® Toolkit —TensorFlow supports CUDA 10.0 (TensorFlow >= 1.13.0)
- CUPTI ships with the CUDA Toolkit.
- cuDNN SDK (>= 7.4.1)
- Tensorflow

__You can visit [Tensorflow website](https://www.tensorflow.org/install/gpu), for installation guide for above requisites.__

## About Dataset

- __The train folder contains images of cat and dogs.The train folder contains 25,000 images of dogs and cats.There are no duplicate images.__
- __The test folder contains 12500 images of cats and dogs.__
- __Each image has been preprocessed to 200x300 pixels.__
- __test Dataset in unlabelled.__<br>
__URL for dataset : https://www.kaggle.com/c/dogs-vs-cats/data__

## About Model

- I have used Convolutional Neural Network to classify images.
- Here is the architecture of the model.
- ![CNN Architecture](https://github.com/kushagra414/Cats-Vs-Dogs/blob/master/screenshots/CNN_model._Architecture.PNG)<br />
- The model has loss: 0.4236, acc: 0.8109,  validation loss: 0.4639 - validation acc: 0.7810
- This could be imporved by increasing the number of epochs from 6 to 10 or higher.
- After Training I saved the model so that I could use it without training the model again and again
- Refer to Cat Vs Dog.ipynb to checkout all the details and code.

## Cats VS Dogs GUI

- I developed the GUI using Python inbuilt module Tkinter.

![Starting Gui](https://github.com/Visurus/CatsVSDogs-Classification/blob/master/CatsVSDogs%20GUI.png?raw=true)<br />
__GUI of the Application__

- There are 2 buttons on the window
  - Upload an image - This button can be used if you want to select an image.
  
  - Classify Image - This Button is used after selecting an image files.
  
  ## Preprocess Images

- To show real-time results to used I implemented preprocessing of images so that the algorithm is able to work on all image sizes.
- Every image is reshaped to 128x128 resizing.

## Executing the model

- First make sure that all the pre-requisites are installed in your computer.
- Then execute the 'CatsVsDogs GUI.py' using :-<br  />
`python3 gui.py'
