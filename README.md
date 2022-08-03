# Multi_Input_NN_Structured_Data

The goal of this project is to build a Keras model automatically based on the structure of the input data. The model is built up layer by layer based on the category of the input columns.

## Data:

The data used in this project comes from a Kaggle competition.

https://www.kaggle.com/competitions/two-sigma-connect-rental-listing-inquiries/overview

The reason for the election is due to the multiple variable types included.

## Requirements:

```pandas:``` Data analysis and manipulation tool.

```spacy:``` is an open-source software library for advanced natural language processing.

```string:``` Common string operations module.

```re:``` This module provides regular expression matching operations

```nltk:``` The Natural Language Toolkit is a suite of libraries and programs for symbolic an statistical natural language processing (NLP).

```keras:``` Open-source software library that provides a Python interface for artificial neural networks. Keras acts as an interface for the TensorFlow library

```scikit-learn:``` Machine Learning library.

## Description: 

### First part: Preprocess and data cleansing. 

After dealing with outliers and some minor issues, text variables are processed. The description variable has been processed using common preprocessing steps and several custom functions tailored to specific needs. The feature variable has not been preprocessed, each feature represents a token.

Once the preprocessing stage is complete, a function is used to transform the data frame into the tensor format required by the Keras model.

### Second part: Deep Learning solution. 

The solution presented is a Multi-input Neural Network created with the Keras Functional API. As mentioned before, the model is built up layer by layer based on the category of the input columns. The following diagram shows the layers added for each type of variable:

<img src="https://user-images.githubusercontent.com/20369543/182665740-babbcef1-3603-4b12-ba7a-6bd4f5f81fa2.PNG" width="600">

