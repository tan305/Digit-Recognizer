# Digit Recognizer

## Problem Definition
MNIST ("Modified National Institute of Standards and Technology") is the de facto “hello world” dataset of computer vision. Since its release in 1999, this classic dataset of handwritten images has served as the basis for benchmarking classification algorithms. As new machine learning techniques emerge, MNIST remains a reliable resource for researchers and learners alike.

In this competition, your goal is to correctly identify digits from a dataset of tens of thousands of handwritten images. We’ve curated a set of tutorial-style kernels which cover everything from regression to neural networks. We encourage you to experiment with different algorithms to learn first-hand what works well and how techniques compare.

## Training Data
The data files train.csv and test.csv contain gray-scale images of hand-drawn digits, from zero through nine.

Each image is 28 pixels in height and 28 pixels in width, for a total of 784 pixels in total. Each pixel has a single pixel-value associated with it, indicating the lightness or darkness of that pixel, with higher numbers meaning darker. This pixel-value is an integer between 0 and 255, inclusive.

The training data set, (train.csv), has 785 columns. The first column, called "label", is the digit that was drawn by the user. The rest of the columns contain the pixel-values of the associated image.

## CNN Model Description
CNN model having similar structure to LeNet5 model with an added layer was used for classification process. The model was developed on Keras Framework using TensorFlow backend. The prediction accuracy of model without regularization was around 98% on the test set but was not able to reach human level performance as it overfitted the training set data. Dropout regularisation and batch normalization was used to address the issue of overfitting and increase the prediction score. The regularised model performed better than the other model and was able to get 99.285% prediction accuracy

## Conclusion
The model was able to gain close to human-level performance on the handwritten digit recognition task.
Dropout or L2 regularisation can be effective for models that are overfitting on the training data and are performing poorly on the validation and test set. 
Batch normalization can also be used to increase the prediction accuracy of our model.
