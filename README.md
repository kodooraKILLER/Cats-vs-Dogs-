# Cats-vs-Dogs
### Project Aim: 
To fully understand the concepts of image processing and computer vision
### Description:
Cats_vs_dogs is a classic system that intelligently classifies cats and dogs based on images. The system is developed using supervised machine learning algorithms. A set of 2000 cat-and-dog annotated images were imported from the Kaggle database and the model was trained with these images.
### Model:
* DataGenerators and Data Augmentors to preprocess the data for the image processing model
* 150x150 image dimension with RGB-3 color system is taken as input tensors.
* 6 Block CNN base derived from ImageNet model. The first 5 layers are frozen, and the topmost CNN block is de-freezed to allow fine tuning upon the given dataset
* 2 layer DENSE model with relu and sigmoid activation.
* Binary output 0/1, with RMSprop optimizer and binary_crossentropy loss function.
* Compiled and trained for 100 epochs over 1000 train data, 500 validation data an 500 test data images.
### Result:
Accuracy: 97.2%
Loss: 0.0048

