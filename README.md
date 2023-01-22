# binaryClassification_practice
Classifying movie reviews into positive or negative categories.

# Introduction
This notebook uses the review text to classify movie reviews into positive or negative categories. It's a two-class classification, or binary classification, which is an important and common kind of machine learning problem.

The main goal of this task is to find a reliable way to evaluate the performance of the model so that the relationship between optimization and generalization, underfitting and overfitting could be monitored and observed, i.e, to find a balance in the tension.

Note: the results of Min.V.Loss and Max.V.Acc in the Performance on Validation Set comparison chart: can not be rendered in exported html format, for more details, please check the notebook.

# Methodology
## Overview
### Feasibility
The IMDB dataset is from the nternet Movie Database (IMDB), which contains 50,000 movie review texts, half for training and half for testing. They contain an equal number of positive and negative reviews. It also has both reviews and labels which meet the conditions of training. This notebook uses tf.keras, which is a high-level API for building and training models in Tensorflow. The imdb datasets comes packaged with Keras, and it has already been turned into sequences of integers. This enables us to focus on model building, training, and evaluation.

The problem is to classify positive and negative movie reviews, therefore it's two-class classification - each input sample should be classified into two mutually opposing categories.

### Workflow
Input preparation:

- Load dataset and understand the date structure
- Vectorize the data: convert lists into tensors

Model building:

- Build a basic model that has statistical power

Validating the approach:

- Use a validation set to monitor the accuracy of the model during training.

Developing a model that overfits:

- Scale up the model

Hyperparameter tunning:

- Learning rate, momentum, batch size
- Regularization: dropout layers, l1/l2/l1_l2 regularization method
- Grid search/random search

Retrain:

- Retrain with entire training set and evaluate on the unseen test set

Conclusion:

- Summarize the training observation
