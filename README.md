# Bike Sharing Assignment
> Building a Linear Regression model to identify the significant variables in predicting the demand for shared bikes


## Table of Contents
* [General Info](#general-information)
* [Technologies Used](#technologies-used)
* [Conclusions](#conclusions)


## General Information
This is an assignment in which we use Keras to build a Neural Network.

In this project, we need to a CNN based model which can accurately detect melanoma. Melanoma is a type of cancer that can be deadly if not detected early. It accounts for 75% of skin cancer deaths. A solution that can evaluate images and alert dermatologists about the presence of melanoma has the potential to reduce a lot of manual effort needed in diagnosis.

We use the `Melanoma dataset` (link)[https://drive.google.com/file/d/1xLfSQUGDl8ezNNbUkpuHOYvSpTyxVhCs/view?usp=sharing] to build the model.

## Summary
Those are the summary retrieved from the model, further information can be found in the Notebook

We built the model using CNN with 3 convolutional layers following by a fully connected layer before going to softmax layer
- The first model has the training accuracy is 87% validation accuracy is just around 54%, it seems to overfit
- The second model has the tensorflow augmenting method applied (`RandomFlip`, `RandomRotation`, `RandomZoom`), the overfitting problem is gone but the model is underfit after 20 epochs
- The final model used the `Augmentor` library to deal with data imbalancing, the result is better with 95% training accuracy and 78% validation accuracy after 50 epochs


## Technologies Used
- `python` - version 3.10
- `pandas` - version 1.5.2
- `notebook` - version 6.5.2
- `matplotlib` - version 3.6.2
- `tensorflow` - version 2.10.1
- `Augmentor` - version 0.2.10

## Contact
Created by [@phucanthony] - feel free to contact me!