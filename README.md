
# Twitter Sentiment Analysis

This project focuses on sentiment analysis using a dataset of tweets. The project includes text preprocessing, feature extraction, and classification using various machine learning models.

## Table of Contents

- [Dataset](#dataset)
- [Preprocessing](#preprocessing)
- [Feature Extraction](#feature-extraction)
- [Model Training](#model-training)
- [Results](#results)
- [Installation](#installation)
- [Usage](#usage)
- [Contributing](#contributing)

## Dataset

The dataset used for this project contains tweets with sentiment labels. For learning purposes, a subset of 500 rows was manually created and used.

## Preprocessing

1. **Loading Data**: The dataset is loaded using Pandas.
2. **Text Cleaning**: Removing stopwords and patterns like "@user_name".
3. **Stemming**: Applied stemming to the text and created a new column for stemmed text.
4. **Lemmatization**: Applied lemmatization to the text and created a new column for lemmatized text.

## Feature Extraction

For both stemmed and lemmatized text, the following feature extraction techniques were used:
1. **Bag of Words (BoW)**
2. **Term Frequency-Inverse Document Frequency (TF-IDF)**
3. **N-grams**: Used unigrams and bigrams.

## Model Training

The following classifiers were trained using each feature extraction method for both stemmed and lemmatized text:

1. **Support Vector Machine (SVM)**
2. **Logistic Regression**
3. **Naive Bayes**

## Results

The performance of each classifier was evaluated using the different feature extraction methods. The models trained include:
- BoW with stemmed text: SVM, Logistic Regression, Naive Bayes
- TF-IDF with stemmed text: SVM, Logistic Regression, Naive Bayes
- N-grams with stemmed text: SVM, Logistic Regression, Naive Bayes
- BoW with lemmatized text: SVM, Logistic Regression, Naive Bayes
- TF-IDF with lemmatized text: SVM, Logistic Regression, Naive Bayes
- N-grams with lemmatized text: SVM, Logistic Regression, Naive Bayes

## Installation

To run the project, you'll need to install the following libraries:
```bash
pip install pandas numpy sklearn nltk wordcloud
```

## Usage

1. Clone the repository:
```bash
git clone https://github.com/yourusername/twitter-sentiment-analysis.git
```
2. Navigate to the project directory:
```bash
cd twitter-sentiment-analysis
```
3. Run the script:
```bash
python sentiment_analysis.py
```

## Contributing

Contributions are welcome! Please create an issue or submit a pull request.
