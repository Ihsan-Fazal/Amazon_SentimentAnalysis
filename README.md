# Amazon Employee Experience & Workplace Culture Analysis
## Overview
This project investigates employee sentiment and workplace culture at Amazon through large-scale analysis of public employee reviews and discussions. By combining data from multiple online platforms, the study explores how employees perceive workplace conditions, management practices, job satisfaction, and operational challenges.

The project applies a complete Natural Language Processing (NLP) pipeline, including data collection, sentiment labeling, feature engineering, machine learning, transformer-based classification, and visualization. The goal is not only to classify sentiment but also to uncover key themes and workplace factors influencing employee experiences.

## Objectives
- Collect and integrate employee reviews from multiple public sources.
- Analyze workplace culture and employee satisfaction at Amazon.
- Compare lexicon-based, machine learning, and transformer-based sentiment classification approaches.
- Evaluate the effectiveness of different text preprocessing and feature representation techniques.
- Visualize sentiment trends and identify recurring workplace themes.

## Data Collection
Employee feedback was collected from multiple sources to ensure diverse perspectives:

- YouTube employee reviews and discussions
- InHerSight workplace reviews
- CareerBliss employee reviews
- Breakroom UK employee reviews

Data was gathered using a combination of:

- YouTube Data API
- Selenium Web Scraping
- Internal API extraction
- JSON-LD metadata extraction

The final dataset contains thousands of employee reviews covering warehouse operations, workplace safety, management, compensation, employee wellbeing, and overall job satisfaction.

## Sentiment Labeling & Validation
To create a labeled dataset, multiple sentiment analysis approaches were evaluated such as TextBlob and VADER Sentiment Analyzer. Performance was benchmarked against manually labeled samples, with VADER selected as the primary labeling approach due to superior Accuracy and Macro F1 performance.

## Text Analytics Pipeline
### Text Preprocessing
The preprocessing pipeline included:
- Lowercasing
- Punctuation removal
- Text normalization
- Tokenization
- Stop-word removal with negation preservation
- Lemmatization
- Feature Representation

Several feature engineering techniques were explored:
- TF-IDF
- N-grams
- Sparse vector representations

These representations were used to transform textual reviews into machine-readable numerical features.

## Machine Learning Models
Traditional machine learning models including Logistic Regression, Multinomial Naive Bayes, and Random Forest were trained and evaluated using TF-IDF features. Hyperparameter tuning and five-fold cross-validation were performed for model optimization.

### Evaluation metrics included:
- Accuracy
- Precision
- Recall
- Macro F1 Score
- Confusion Matrix Analysis
Five-fold cross-validation was used to provide reliable estimates of model generalization performance.

### Transformer-Based Modelling
To compare traditional NLP approaches with modern language models, DistilBERT was fine-tuned for sentiment classification. DistilBERT was selected due to its strong performance while remaining computationally efficient.

## Visualization & Insights
Exploratory data analysis and sentiment visualization were used to identify:
- Overall sentiment distribution
- Frequently occurring workplace concerns
- Positive and negative employee themes
- Workplace culture indicators
The visual analysis provided insights into employee perceptions of management, workload, safety, communication, and workplace satisfaction.

## Key Outcomes
- Built a multi-source employee sentiment dataset.
- Compared lexicon-based and machine learning sentiment classification approaches.
- Evaluated transformer-based models for workplace sentiment analysis.
- Identified recurring themes influencing employee satisfaction and dissatisfaction.
- Generated actionable insights into Amazon's workplace culture through NLP and visualization techniques.

## Languages & Libraries
- Python
- Pandas
- NumPy
- NLTK
- Scikit-learn
- Selenium
- YouTube Data API
- TextBlob
- VADER
- Hugging Face Transformers
- DistilBERT
- Matplotlib
- Seaborn

## Contributors
| [`Ihsan-Fazal`](https://github.com/Ihsan-Fazal)|
| [`Vaishnavi-chintha`](https://github.com/Vaishnavi-chintha)|
| [`Mohamed Hafeez`](https://github.com/mhd-hfz)|
