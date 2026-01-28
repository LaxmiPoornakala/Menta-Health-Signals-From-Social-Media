# Mental Health Signals from Social Media

## Overview

This project analyzes large-scale publicly available social media data to identify linguistic and emotional patterns associated with stress and mental health signals.

Using Natural Language Processing (NLP) and statistical modeling techniques, the system processes ~550,000+ social media posts to extract sentiment, emotion, and psycholinguistic features for analytical and predictive modeling.

> ⚠️ Note: This project uses publicly available datasets from Mendeley and Kaggle. All data is de-identified and non-clinical. No protected health information (PHI) or medical records were used.

## Objective

To detect and analyze stress-related patterns in online text using:

- Sentiment analysis  
- Emotion lexicons  
- Psycholinguistic feature extraction  
- Statistical correlation and predictive modeling  

## Data Sources

- Public Reddit / Twitter (X) datasets  
- Public behavioral survey datasets  
- Non-clinical, non-identifiable data  

Total dataset size: **~550,000+ posts**

## Methodology

### 1 Data Processing Pipeline
- Text cleaning (URLs, punctuation, stopwords removal)
- Tokenization & lemmatization
- Normalization
- Feature scaling

### 2 Feature Engineering
- LIWC psycholinguistic features  
- NRC Emotion Lexicon features  
- Sentiment polarity scoring  
- Word frequency-based metrics  

### 3 Exploratory Data Analysis (EDA)
- Stress vs non-stress distribution analysis  
- Emotional intensity comparisons  
- Correlation analysis (R² ≈ 0.89 in experiments)  
- Trend visualization  

### 4 Modeling & Evaluation
- Regression analysis  
- Binary classification (stress vs non-stress)  
- Evaluation metrics:
  - Accuracy  
  - Precision  
  - Recall  
  - F1-score  

## Key Insights

- Strong correlation between stress signals and negative emotional language.
- Certain linguistic markers consistently predicted elevated stress likelihood.
- Emotion-based features significantly improved predictive performance.
- Sentiment polarity effectively differentiated stress and non-stress groups.

## Tech Stack

- Python  
- Pandas  
- NumPy  
- scikit-learn  
- Matplotlib / Seaborn  
- NLTK / spaCy  
- LIWC & NRC Emotion Lexicons  

## How to Run

1. Install dependencies:
```bash
pip install pandas numpy scikit-learn matplotlib seaborn nltk spacy
```

2. Download required NLP models:
```bash
python -m nltk.downloader all
```

3. Run the Jupyter notebooks to reproduce analysis and modeling.

## Skills Demonstrated

- Large-scale unstructured data processing
- NLP preprocessing pipelines
- Feature engineering
- Statistical analysis & correlation modeling
- Predictive modeling
- Data visualization & storytelling