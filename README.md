Movie Genre Classifier Using k-Nearest Neighbors (k-NN)

This project uses machine learning techniques to classify movies into genres based on their screenplay text, represented in a bag-of-words format. 

Project Overview
The primary goal of this project is to develop a classifier that predicts whether a movie belongs to the "comedy" or "thriller" genre based on its screenplay. 
This involves implementing and evaluating the k-nearest neighbors (k-NN) algorithm while applying various data analytic and feature engineering techniques.

Techniques Used:
1. Sampling:
   Randomly split the dataset into training (85%) and test (15%) subsets.
   Stratified sampling to preserve genre proportions.

2. k-Nearest Neighbors (k-NN):
   Implemented a classifier that calculates the Euclidean distance between movies based on selected word features.
   Used k = 13 for optimal classification accuracy.

3. Performance Evaluation:
   Tested the model's accuracy on unseen test data.
   Analyzed misclassified movies to identify patterns and refine the feature set.

How It Works:

1. Data Preprocessing: Convert raw word counts to proportions relative to the total words in a movie.
Stem words to group similar terms (e.g., "manage", "managed", "managerial").


2. Model Training: Train the k-NN model using a subset of movies with known genres.
Calculate distances between movies based on their word frequencies.
Classification:

3. For each test movie, find the k nearest neighbors from the training set.
Classify the movie based on the majority genre among its neighbors.
Evaluation:

4. Measure the model's accuracy on the test dataset.

