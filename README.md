# Disaster Tweet Classification

## Project Overview

In this project, we tackled the challenge of classifying tweets to determine whether they are related to real disasters or not. This task is crucial as it helps disaster relief organizations and news agencies quickly identify and act on emergency situations announced on Twitter. The competition dataset consists of tweets labeled as disaster-related or not, which we used to train and evaluate a machine learning model.

## Dataset Description

- **Train Set:** Contains tweets and their labels indicating whether they are about disasters (1) or not (0).
- **Test Set:** Contains tweets for which predictions need to be made.

## Data Preprocessing

1. **Text Cleaning:**
   - **Lowercasing:** All tweets were converted to lowercase to standardize the text data.
   - **Stopwords Removal:** Commonly used words (stopwords) were removed to focus on the significant words in the tweets.
   - **Stemming:** Words were reduced to their root form to ensure that variations of words are treated as the same feature.

2. **Feature Extraction:**
   - **TF-IDF Vectorization:** We used Term Frequency-Inverse Document Frequency (TF-IDF) to convert the text data into numerical features. This approach helps capture the importance of words in the context of the dataset.

## Model Training

- **Logistic Regression:** We employed Logistic Regression, a fundamental classification algorithm, to predict whether a tweet is related to a disaster. 
- **Hyperparameter Tuning:** Using Grid Search Cross-Validation, we tuned the hyperparameter `C`, which controls the regularization strength, to optimize model performance.

## Evaluation

- **Confusion Matrix:** We evaluated the model using confusion matrices to visualize the performance and understand the distribution of true positives, true negatives, false positives, and false negatives.
- **F1 Score:** The F1 score, which balances precision and recall, was used to assess the overall performance of the model.

## Final Model and Submission

After training and evaluating the model, it was retrained on the full training dataset using the best hyperparameters. Predictions were made on the test set, and the results were saved in a CSV file for submission.

## Acknowledgements

- **Dataset Source:** This dataset was created by figure-eight and shared on their 'Data For Everyone' website.
- **Tweet Source:** [Tweet Example](https://twitter.com/AnyOtherAnnaK/status/629195955506708480).

## Contact

For questions or discussions related to this project, please join the Kaggle competition's [Discord community](https://discord.gg/kaggle).
