# Sentiment Analysis of Flipkart Reviews

This Python project performs sentiment analysis on Flipkart product reviews using various libraries and tools including `pandas`, `numpy`, `nltk`'s `SentimentIntensityAnalyzer`, `wordcloud`, `seaborn`, and `matplotlib.pyplot`. The goal is to analyze and visualize the sentiment distribution of reviews for a better understanding of customer opinions.

## Table of Contents

- [Importing libraries](#importing-libraries)
- [Data Preparation](#data-preparation)
- [Sentiment Analysis](#sentiment-analysis)
- [Data Visualization](#data-visualization)
- [Contributing](#contributing)

## Importing libraries

To start with the project we need to import all the necessary libraries needed . 

```bash
import pandas as pd
import seaborn as sns
import matplotlib.pyplot as plt
from nltk.sentiment.vader import SentimentIntensityAnalyzer
from wordcloud import WordCloud, STOPWORDS, ImageColorGenerator
```

## Data Preparation

Before performing sentiment analysis, you need to collect Flipkart reviews data. You can manually copy and paste reviews from the Flipkart website into a CSV file or use web scraping techniques to automate data collection. Ensure that the CSV file has at least the following columns:

- `Review Text`: The text of the review.
- `Rating`: The numerical rating given by the user (e.g., 1-5).

![image](https://github.com/riddle-me/Sentiment-analysis-on-Flipkart-reviews-/assets/124533399/95ecac1e-3ab9-4859-b33f-e509d811d2b8)

## Sentiment Analysis

The sentiment analysis is performed using the `SentimentIntensityAnalyzer` from the NLTK library. It assigns sentiment scores to each review, indicating whether the review is positive, negative, or neutral. The script calculates the following sentiment scores for each review:

- **Compound Score**: A normalized compound score ranging from -1 (most negative) to 1 (most positive).
- **Positive Score**: The positive sentiment score.
- **Negative Score**: The negative sentiment score.
- **Neutral Score**: The neutral sentiment score.

The script then classifies each review as either positive, negative, or neutral based on the compound score.

## Data Visualization

After performing sentiment analysis, the script generates various visualizations using `wordcloud`, `seaborn`, and `matplotlib.pyplot`. These visualizations include:

- **Word Cloud**: A word cloud visualization of the most frequently occurring words in positive and negative reviews.
- **Sentiment Distribution**: A bar chart showing the distribution of sentiment (positive, negative, neutral) in the reviews.
- **Rating vs. Sentiment**: A box plot showing the relationship between product ratings and sentiment.

## Contributing

If you'd like to contribute to this project, please fork the repository and create a pull request. You can also open issues for bug reports or feature requests.
