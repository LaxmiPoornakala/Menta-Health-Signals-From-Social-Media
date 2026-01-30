# Mental Health Signals from Social Media

## Overview

This project analyzes large-scale public social media and survey datasets to identify linguistic and behavioral indicators associated with stress and mental health outcomes.

Using R-based NLP, statistical modeling, and machine learning techniques, the project combines:

- Text-based stress detection (Dreaddit dataset)
- Emotion & sentiment analysis (Mendeley Twitter dataset)
- Behavioral validation (Students, Bhavik, and SMMH datasets)

> Note: All datasets are publicly available and de-identified research data. No clinical records or protected health information were used.

## Objectives

- Detect stress-related patterns in social media text
- Compare machine learning classifiers for stress prediction
- Validate findings using independent behavioral datasets
- Analyze relationships between digital behavior and mental health metrics

## Data Sources

- Dreaddit stress dataset  
- Mendeley Twitter dataset  
- Students Social Media Addiction dataset  
- Bhavik Mental Health dataset  
- SMMH (Social Media & Mental Health) dataset  

Total processed data: ~550,000+ text records + survey datasets

## Methodology

### 1 Text-Based Stress Classification (Dreaddit)

- Removed raw text leakage columns
- Applied preprocessing (imputation, scaling, NZV filtering)
- Performed train/test split (80/20)
- Used SMOTE for class balancing
- Compared multiple classifiers:

  - Logistic Regression (GLM)
  - Random Forest
  - SVM (Radial)
  - XGBoost
  - Naive Bayes

- Evaluation metrics:
  - Accuracy
  - F1 Score
  - AUC
  - ROC curves
  - Confusion matrices
  - Feature importance

### 2 Emotion & Sentiment Analysis (Twitter Data)

- Cleaned tweets (URLs, mentions, punctuation removal)
- Applied NRC emotion lexicon via `syuzhet`
- Computed:
  - Stress score (sadness + fear + anger + disgust)
  - Positive score (joy + trust + anticipation + surprise)
- Generated:
  - Sentiment distribution plots
  - Stress score histograms
  - Stress vs sentiment regression analysis
  - Emotion radar charts (Stress vs Non-Stress)

### 3 Behavioral Validation (Survey Datasets)

#### Students Dataset
- Correlation: social media usage vs mental health score
- Linear regression modeling
- Observed vs fitted validation plots
- Correlation heatmap

#### Bhavik Dataset
- Logistic regression on treatment-seeking behavior
- Odds ratio estimation with confidence intervals

#### SMMH Dataset
- Created composite distress index
- Correlation: time spent vs distress index
- Regression modeling

## Key Findings

- Stress-related language strongly correlates with negative emotion intensity.
- Ensemble models (RF, XGBoost) outperformed baseline GLM.
- Increased social media usage correlates with reduced mental health scores.
- Emotional distress indicators significantly predict treatment-seeking behavior.
- Behavioral survey results align with text-based stress detection findings.

## Tech Stack

- R
- data.table
- tidyverse
- caret
- pROC
- tm
- syuzhet
- xgboost
- kernlab (SVM)
- naivebayes
- ggplot2
- fmsb (radar charts)

## How to Run

1. Install required packages in R.
2. Place datasets inside `/Data` directory.
3. Run the R Markdown / script file sequentially.

## Skills Demonstrated

- NLP preprocessing in R
- Emotion lexicon analysis
- Feature engineering
- Model comparison & evaluation
- SMOTE handling for imbalanced data
- Statistical modeling (linear & logistic regression)
- Behavioral data validation
- Advanced data visualization

## License

Academic / Research Project