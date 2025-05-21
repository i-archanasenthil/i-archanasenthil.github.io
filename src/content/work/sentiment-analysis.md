---
title: Sentiment Analysis
publishDate: 2025-02-22 00:00:00
img: /assets/sentiment.jpg
img_alt: Iridescent ripples of a bright blue and pink liquid
description: |
  Performed sentiment analysis on tweets from multiple Twitter accounts to classify them as positive, negative, or neutral. Generated word clouds to visualize the most frequent and sentiment-representative terms.
tags:
  - Sentiment Analysis
  - Natural Language Processing
  - Word Cloud
  - Polarity Analysis
  - Social Media Monitoring
---

This project explores sentiment analysis of tweets collected from various Twitter accounts, aiming to understand public opinion and emotional tone conveyed through short-form social media content. Using natural language processing (NLP) techniques, tweets were first collected via the Twitter API and then cleaned through a series of preprocessing steps. These included lowercasing, removing punctuation, hyperlinks, mentions, hashtags, stopwords, and irrelevant characters—resulting in a clean corpus ready for analysis.

The cleaned text data was analyzed using a sentiment classification model that assigns each tweet a label—positive, negative, or neutral. This classification helped quantify and categorize the emotional tone expressed by different users or in response to different events or topics. The sentiment results were aggregated and visualized to observe distribution patterns and identify trends across accounts.

In addition to sentiment classification, a word cloud was generated using the full corpus of cleaned tweets. This visualization highlights the most frequently used words, offering insight into common themes and topics being discussed by users, independent of sentiment. The word cloud serves as an accessible, high-impact way to identify dominant vocabulary and recurring ideas in social media content.

Overall, this project demonstrates how simple but effective text mining techniques can be used to perform social media listening, highlight key narratives, and support real-time opinion tracking through visual and analytical means.

🔗 GitHub Repository: [Sentiment Analysis on Tweets](https://github.com/i-archanasenthil/sentiment-analysis-tweets-LDA)