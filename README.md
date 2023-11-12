# tweet_sentiment_analysis
This code performs sentiment analysis on a dataset of tweets. Here is a summary of what each section of the code does:

1. Importing Libraries: Import necessary libraries for data manipulation, visualization, and machine learning using Keras and TensorFlow. Also, set up the environment for inline plotting.

Loading Data: Read a CSV file containing tweet data into a Pandas DataFrame and display basic information about the dataset, such as the columns, data types, and non-null counts.

Clean the Data: Check for and handle missing values in the dataset.

Generate X Values by Sentence Vector & Text Normalization:

Clean the sentences by removing special characters, converting to lowercase, and identifying potential insults.
Create a new column ('filtered_text') in the DataFrame with the cleaned sentences.
Sentence Vector with Tokenizer:

Tokenize the cleaned text and convert it into sequences.
Pad the sequences to ensure consistent length.
Create Sentiment's Vector Column, Y:

Convert the categorical sentiment labels into numerical values and one-hot encode them.
First Model Fitting and Predicting:

Split the data into training and testing sets.
Build a simple LSTM (Long Short-Term Memory) neural network model using Keras.
Train the model on the training data and evaluate it on the test data.
Model Optimization:

Search for the best hyperparameters using GridSearchCV, including hidden nodes, dropout rate, optimizer, batch size, and epochs.
Train a new model with the optimized hyperparameters.
Conclusion:

Evaluate the final model on the test set and compare the performance with the initial model.
Define a function to make predictions on new sentences using the trained model.
Test Predictions:

Use the trained model to predict the sentiment of some example sentences.
The code demonstrates the process of building, optimizing, and evaluating a sentiment analysis model for tweets using LSTM neural networks.
