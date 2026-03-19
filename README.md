#  Fake News Detection System

### Purpose
The objective of this project is to develop a classification system capable of distinguishing between factual reporting and misinformation (fake news). By applying natural language processing (NLP) and statistical analysis, the system identifies patterns in writing style, emotional bias, and structural anomalies that characterize deceptive content.

The primary goal is to provide a quantitative credibility score for any given text, moving beyond simple keyword matching toward a deeper understanding of linguistic intent.

---

### Core Features

#### 1. Multidimensional Text Analysis
The system analyzes news articles through two distinct lenses:
* **Semantic Context:** Evaluating the actual meaning, narrative flow, and relationship between words to detect subtle misinformation.
* **Stylometric Profiling:** Quantifying structural patterns such as punctuation density, capitalization ratios, and average sentence length—metrics that often vary significantly between professional journalism and "clickbait."

#### 2. Automated Data Preprocessing Pipeline
To ensure high-quality input for the model, the project includes a standardized pipeline for:
* **Noise Reduction:** Removal of irrelevant characters, HTML tags, and stop-words.
* **Text Normalization:** Implementing lemmatization and tokenization to reduce words to their core linguistic roots.
* **Feature Scaling:** Preparing numerical metadata for integration with text-based vectors.

#### 3. Sentiment and Bias Quantification
The project incorporates sentiment analysis to detect "loaded language." By measuring the intensity of emotional triggers within an article, the system can flag content that prioritizes emotional manipulation over factual reporting.

#### 4. Probabilistic Credibility Rating
The output is a continuous probability score rather than a simple binary classification. This allows for a nuanced assessment of content that may contain "partial truths" or highly biased reporting.

#### 5. Performance Benchmarking
Evaluation is focused on high-precision metrics to minimize the "False Positive" rate (incorrectly flagging legitimate news). Success is measured using:
* **Precision-Recall Curves**
* **F1-Score**
* **Confusion Matrix Analysis**
