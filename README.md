# Kindle Review Sentiment Analysis

This project performs sentiment analysis on a subset of Amazon Kindle Store book reviews. The goal is to classify reviews as positive or negative using various NLP techniques and machine learning algorithms.

## Dataset

- **Source:** [Amazon product data, Julian McAuley, UCSD](http://jmcauley.ucsd.edu/data/amazon/)
- **Description:** 5-core dataset of product reviews from the Kindle Store (May 1996 - July 2014), with 982,619 entries. Each reviewer and product has at least 5 reviews.
- **Columns:**
  - `asin`: Product ID
  - `helpful`: Helpfulness rating
  - `overall`: Product rating
  - `reviewText`: Review text
  - `reviewTime`: Review time
  - `reviewerID`: Reviewer ID
  - `reviewerName`: Reviewer name
  - `summary`: Review summary
  - `unixReviewTime`: Unix timestamp

## Project Steps

1. **Preprocessing and Cleaning**
   - Lowercasing, removing special characters, stopwords, URLs, HTML tags, and extra spaces
   - Lemmatization

2. **Train-Test Split**
   - Splitting the dataset into training and testing sets

3. **Feature Extraction**
   - Bag of Words (BoW)
   - TF-IDF
   - (Word2Vec placeholder)

4. **Model Training**
   - Gaussian Naive Bayes classifier

5. **Evaluation**
   - Confusion matrix and accuracy score

## Requirements

- Python 3.x
- pandas
- numpy
- scikit-learn
- nltk
- gensim
- beautifulsoup4

Install dependencies with:

```sh
pip install pandas numpy scikit-learn nltk gensim beautifulsoup4
```

## Usage

1. Place the dataset CSV file in the `Kindle Reviews/` directory as `all_kindle_review.csv`.
2. Run the Jupyter notebook:  
   ```
   jupyter notebook "Kindle Review Sentiment Analyis.ipynb"
   ```
3. Follow the notebook cells to preprocess data, train models, and evaluate results.

## Acknowledgements

- Dataset from [Julian McAuley, UCSD](http://jmcauley.ucsd.edu/data/amazon/)

## License

This project is for educational purposes. Dataset license belongs to
