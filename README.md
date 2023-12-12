# Tweet Classification: Trump vs. Trudeau

## Overview
This project focuses on classifying tweets from two prominent North American politicians: Donald Trump and Justin Trudeau. The goal is to explore the challenges of text classification on social media data, particularly tweets, and build a classifier to distinguish between the two tweeters.

## Tools and Libraries
The project uses Python and scikit-learn for natural language processing (NLP) tasks. The following tools and libraries are utilized:
- CountVectorizer and TfidfVectorizer for text vectorization.
- MultinomialNB (Naive Bayes), LinearSVC, and PassiveAggressiveClassifier for classification.
- Train-test split, GridSearchCV, and metrics from scikit-learn for model evaluation.
- Pandas for data manipulation.

## Project Structure
1. **Tweet Collection and Data Preparation**
    - The project starts with a corpus of tweets collected in November 2017.
    - The data is loaded into a Pandas DataFrame and split into training and testing sets.

2. **Text Vectorization**
    - The tweets are vectorized using CountVectorizer and TfidfVectorizer.
    - Vectorization is a crucial step in preparing the data for machine learning models.

3. **Model Training**
    - Two models are trained: Multinomial Naive Bayes and Linear Support Vector Classifier (LinearSVC).
    - Model performance is evaluated using accuracy scores.

4. **Confusion Matrix**
    - The confusion matrix is used to analyze the model's performance in detail.
    - True Positives, False Positives, False Negatives, and True Negatives are considered for each class.

5. **Top Features**
    - The LinearSVC model's top features (important tokens) are introspected and displayed.
    - This provides insights into what words contribute most to classifying tweets as Trump or Trudeau.

6. **Bonus: Write Your Own Tweet**
    - Users can challenge the model by writing tweets to see if they can fool the classifier.
    - French words are identified as important features for Trudeau.

## Future Work
- Additional preprocessing steps (e.g., removing URLs or French stop words) can be explored to improve model performance.
- GridSearchCV can be used for parameter optimization.
- Introspection of the Naive Bayes model to identify words characteristic of Trump or Trudeau.
- Updating the dataset with more recent tweets using tools like Tweepy for retraining.

## How to Run
1. Clone the repository.
2. Install the required dependencies using `pip install -r requirements.txt`.
3. Run the Jupyter Notebook to go through the analysis and classification steps.

Feel free to share your own tweets on Twitter and see if you can trick the model!

Happy coding!
