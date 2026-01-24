# AI-Powered Customer Insight Engine for Beauty Brands

## Overview
As beauty brands release a wide range of makeup products, analyzing thousands of customer reviews manually is no longer scalable. This project implements an **AI-powered review analysis tool** that enables brands to extract structured insights from unstructured customer feedback. 

By combining **RoBERTa (Sentiment Analysis)** and **NMF (Topic Modeling)**, this engine uncovers *what* customers are saying and *how* they feel, helping teams make informed decisions about product improvement and marketing.

## Features
- **Sentiment Classification at Scale**: Uses a RoBERTa language model (`cardiffnlp/twitter-roberta-base-sentiment`) to classify reviews as Positive, Neutral, or Negative.
- **Review Cleaning & Consolidation**: Automatic preprocessing of pros/cons into single opinion statements.
- **Topic Modeling**: Uses Non-negative Matrix Factorization (NMF) to identify latent themes (e.g., texture, packaging, shade match).
- **Insight Generation**: Merges sentiment labels with product metadata (brand, rating) to surface performance shifts and "why" behind the ratings.
- **Streamlit Dashboard**: A prototype interface for visualizing sentiment trends and topic insights.

## Project Structure
- `code files/`: Contains the Jupyter notebooks for the analysis and the Streamlit app.
    - `AI Powered Customer Insight Engine for Beauty Brands.ipynb`: Core logic for sentiment analysis and topic modeling.
    - `Streamlit (1).ipynb`: Code for the dashboard interface.
- `data/`: Datasets used for the project (Customer Reviews and Makeup Products metadata).
- `images/`: Assets used in reports or the dashboard.
- `annotated-BUDT...Final Report.docx.pdf`: Detailed project report.

## Methodologies
1. **Data Preprocessing**: Merging review text, cleaning implementation (regex, lowercase), and consolidating metadata.
2. **Sentiment Analysis**: Applied RoBERTa to 1,000 sampled reviews (93.8% accuracy on positive sentiment).
3. **Topic Modeling**: Vectorized text with CountVectorizer and extracted 5 key themes using NMF.

## Future Scope
- **Bias Mitigation**: Expanding datasets to better represent diverse skin tones and demographics.
- **Real-time API**: deploying the Streamlit app as a live web service.
- **LLM Integration**: Using large language models for automatic summarization of customer pain points.
