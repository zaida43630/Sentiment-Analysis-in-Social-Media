Political Sentiment Analysis in Social Media

📌 Project Overview

This project implements a machine learning pipeline to analyze public political sentiment on social media. By leveraging Natural Language Processing (NLP) techniques, the system automates the classification of YouTube comments into three distinct categories: Pro-Government, Anti-Government, and Neutral.

The tool is designed to monitor public opinion trends effectively, providing a scalable alternative to traditional surveys and polls. It achieves a classification accuracy of 94% using Logistic Regression and TF-IDF vectorization.

🎯 Objectives

Automate Sentiment Analysis: Classify unstructured user-generated content into political sentiment categories.

Data Pipeline: Build a robust pipeline for collecting, cleaning, and preprocessing text data.

Trend Identification: Quantify public support or opposition towards government policies.

High Performance: Deliver accurate predictions even with colloquial or noisy social media text.

🛠️ Tech Stack

Language: Python

Machine Learning: scikit-learn (Logistic Regression, Model Evaluation)

NLP: NLTK (Tokenization, Stopwords, Lemmatization)

Data Handling: Pandas, NumPy

Visualization: Matplotlib, Seaborn

Data Collection: youtube_comment_downloader

Utilities: google_trans (for translating regional comments to English)

📊 Dataset Details

The dataset was constructed specifically for this project by scraping comments from political influencer videos on YouTube.

Total Samples: 1,664 comments

Class Distribution:

1 Pro-Government: 895 comments (Most frequent)

-1 Anti-Government: 449 comments

0 Neutral: 318 comments

Labeling: Manual annotation based on expressed sentiment.

⚙️ Methodology

The project follows a standard supervised learning workflow:

Data Collection: Comments are scraped from relevant YouTube videos using youtube_comment_downloader.

Translation: Non-English comments are translated to English using google_trans to ensure uniformity.

Preprocessing:

Lowercasing text

Removing URLs, punctuation, and special characters

Tokenization and Stopword removal

Lemmatization (reducing words to their base form)

Feature Extraction: Text is converted into numerical vectors using TF-IDF (Term Frequency-Inverse Document Frequency) to highlight unique, significant words.

Model Training: A Logistic Regression classifier is trained on the vectorized data.

📈 Results & Performance

The model demonstrates robust performance across all sentiment classes, with particularly high recall for the majority class.

Metric

Score

Accuracy

94%

Macro F1-Score

0.94

Pro-Gov Recall

98%

Anti-Gov Recall

93%

Key Insight: The model effectively captures the dominant sentiment (Pro-Government) while maintaining high precision for Anti-Government comments, rarely misclassifying them.

🚀 Installation & Usage

Clone the repository:

git clone [https://github.com/yourusername/political-sentiment-analysis.git](https://github.com/yourusername/political-sentiment-analysis.git)
cd political-sentiment-analysis


Install dependencies:

pip install -r requirements.txt


Run the analysis:
(Replace main.py with your actual script name)

python main.py


🔮 Future Scope

Real-Time Dashboard: Develop a live web interface for monitoring sentiment changes over time.

Multilingual NLP: Implement native processing for regional languages to remove the dependency on translation.

Emotion Detection: Expand the model to detect specific emotions (anger, joy, sarcasm) rather than just polarity.

Aspect-Based Analysis: Granular analysis of sentiment towards specific topics (e.g., economy, foreign policy).

👥 Author

Mohd Zaid

Department of Computer Science & Engineering

🙏 Acknowledgements

Special thanks to Dr. Apurbalal Senapati for his guidance and supervision throughout this project.
