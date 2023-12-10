## Project Summary:

This project aims to build a multi-stage model for detecting offensive and hate speech in Twitter data.

**Key steps:**

1. **Data loading and cleaning:**
    * Load data from a CSV file.
    * Clean text data by converting to lowercase, removing URLs, punctuation, digits, and stop words.
    * Handle missing values.
2. **Word2Vec:**
    * Tokenize tweets.
    * Train a Word2Vec model to represent words as vectors.
    * Generate Word2Vec features for each tweet.
    * Train a Random Forest classifier using Word2Vec features.
3. **CountVectorizer and Ensemble Model:**
    * Convert text data to a matrix of token counts using CountVectorizer.
    * Split data into training and testing sets.
    * Train three classifiers (Random Forest, SVM, Logistic Regression).
    * Create an ensemble model using soft voting of the three classifiers.
4. **Decision Tree:**
    * Train a Decision Tree classifier with a specified maximum depth.
5. **XGBoost:**
    * Encode labels.
    * Train an XGBoost classifier.
6. **Prediction Function:**
    * Define a function to predict offensiveness using the ensemble model, Decision Tree, and XGBoost.
7. **Testing and Visualization:**
    * Test the prediction function on example texts.
    * Visualize the Decision Tree.

**Overall, this project utilizes a combination of text cleaning, feature engineering, and ensemble learning to achieve accurate detection of offensive and hate speech in Twitter data.**
