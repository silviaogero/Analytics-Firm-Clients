# Analytics-Firm-Clients

# Customer Reviews Analysis

## Overview

This project analyzes Amazon customer reviews using Natural Language Processing (NLP), time series analysis, and neural networks to explore customer feedback and predict product ratings.

## Objectives

- Preprocess and explore customer review text.
- Identify common words and phrases in reviews.
- Examine monthly review volume and average rating trends.
- Build a neural network to predict ratings from review text.
- Evaluate model performance and identify areas for improvement.

## Dataset

The project uses `amazon_reviews_lab.csv`, containing review text, customer ratings, timestamps, and related information.

**Note:** The dataset is required to run the notebook and is not necessarily included in this repository.

## Technologies Used

- Python
- Pandas and NumPy
- Matplotlib and Seaborn
- NLTK
- Scikit-learn
- Statsmodels
- TensorFlow/Keras

## Methodology

### 1. Natural Language Processing
Review text was cleaned and tokenized. Stop words were filtered while retaining negation terms, and lemmatization was applied. Frequent words and bigrams were then explored.

### 2. Time Series Analysis
Review timestamps were converted and aggregated by month to examine review volume and average customer ratings. Trend patterns and potential stationarity concerns were considered.

### 3. Neural Network Classification
TF-IDF was used to convert review text into numerical features. A neural network was trained to predict one of five rating classes, and its performance was evaluated using accuracy, precision, recall, F1-score, and a confusion matrix.

## Key Results

- Review activity increased substantially after 2009, with fluctuations in later years.
- The rolling average suggested possible improvement in customer ratings toward 2014.
- The neural network achieved **56% test accuracy**.
- Rating 5 was the best-predicted class, while Ratings 2 and 3 were more difficult to classify.
- Class imbalance and overfitting were identified as important model limitations.

## Recommendations

- Investigate common complaints and periods of low customer ratings.
- Address class imbalance and overfitting in future classification models.
- Compare alternative models and evaluate performance across all rating classes.
- Interpret time series findings cautiously when monthly review counts are low.

## How to Run

1. Clone or download the project repository.
2. Install the required Python libraries.
3. Place `amazon_reviews_lab.csv` in the notebook's working directory.
4. Open the notebook in Jupyter Notebook or JupyterLab.
5. Run the cells in order.

## Limitations

The dataset has an imbalanced rating distribution, sparse activity in some months, and limited classification performance for lower ratings. Further testing is needed before using the model for real-world decisions.

## Author

Silvia Ogero
