
# Stock Movement Analysis Based on Social Media Sentiment

# Project Overview
This project is designed to analyze and predict stock price movements by extracting and analyzing data from social media platforms like Reddit. By applying sentiment analysis to discussions about specific stocks, this project aims to offer insights into potential price trends, helping inform buy/sell decisions.

# Objective
The goal of this project is to examine the connection between social media sentiment and stock price fluctuations. Through data scraping, sentiment analysis, and correlating the findings with stock price data, the aim is to uncover useful insights for traders and investors.


# Setup Instructions



## Prerequisites

Make sure that Python (version 3.6 or higher) is installed on your system and that pip is available for managing packages.


## Installation

Clone the repository to your local machine:

```bash
git clone <repository-url>
cd Stock_Sentiment_Analysis
```
Install the required dependencies using `pip`:

```bash
pip install -r requirements.txt
```
 ### Get API Keys

 You will need API keys to access Reddit API:

 ### Reddit API:
- Go to the Reddit App Preferences.
- Click on "Create App" or "Create Another App."
- Fill in the required fields. Select the script option.
- Note the `client_id`, `client_secret`, and `user_agent`.

### Configure API Keys:

REDDIT_CLIENT_ID = `your_reddit_client_id`

REDDIT_CLIENT_SECRET = `your_reddit_client_secret`

REDDIT_USER_AGENT = `your_reddit_user_agent`

Run the data scraping script to collect the required data:
```bash
python scripts/data_scraping.py
```
Open the Jupyter Notebook for analysis:
```bash
jupyter notebook notebooks/Stock_Sentiment_Analysis.ipynb1
```
- Open the notebook and run the cells to perform sentiment analysis and feature extraction.

#### Visualize Results

The notebook contains code for visualizing the results. Run the corresponding cells to generate the visualizations.

### Data Collection
- Input: Raw data from Reddit (e.g., posts from r/wallstreetbets).
- Output: Cleaned dataset containing sentiment scores, post metadata, and stock mentions.

### Analysis and Feature Extraction
- Input: Cleaned data from the scraping step.
- Output:
- Sentiment scores (positive, negative, neutral)
Frequency of mentions
- Additional features for correlation analysis

# Analysis Results

## Visualization
- Input: Results from the analysis step.
- Output: Visualizations (charts, graphs) that show trends in stock sentiment, Frequency of Mentions Over Time and Correlations between sentiment and stock price movements.


## Sentiment Counts
- Neutral Sentiments: 298 occurrences
- Negative Sentiments: 2 occurrences

This shows that the vast majority (about 99.3%) of comments are neutral, with only a small percentage showing negative sentiment.

## Stock Mentions
- Total Mentions of AAPL: 0 mentions

This indicates that there were no mentions of AAPL in the analyzed comments. It might suggest that AAPL isn't a topic of interest in the specific subreddit or threads analyzed.

## Recommendations Based on Findings

- Expand Data Collection: To get a more comprehensive view, consider scraping additional subreddits or posts about stocks or focus on more popular stocks to capture relevant discussions and sentiments.

- Explore Other Stocks: If AAPL isn't being discussed, it could be worthwhile to track discussions about other trending stocks or those currently in the news.

- Evaluate Sentiment Analysis Model: Since most of the sentiment is neutral, reviewing and refining the sentiment analysis model might help improve its sensitivity and accuracy in detecting a wider range of sentiments, particularly positive ones.

- Monitor Trends Over Time: Conducting this analysis over various time periods might help identify trends and shifts in sentiment and stock mentions, which could be linked to stock price movements.






