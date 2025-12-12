# Political Sentiment Analysis in Social Media

## 📌 Project Overview
This project aims to automate the analysis of public opinion trends by classifying YouTube comments into political sentiment categories. [cite_start]Using Natural Language Processing (NLP) and Machine Learning techniques, the system interprets user-generated content to gauge public sentiment towards the government.

## 🎯 Objectives
- [cite_start]**Sentiment Classification:** Categorize comments into **Pro-Government**, **Anti-Government**, or **Neutral**.
- **Data Processing:** Collect, clean, and preprocess raw user-generated text.
- [cite_start]**Trend Analysis:** Identify public opinion trends regarding government policies.

## 📊 Dataset
- [cite_start]**Source:** Comments collected from videos of prominent political influencers on YouTube.
- [cite_start]**Size:** 1,664 comments.
- **Labeling:** Manually labeled into three classes:
  - [cite_start]`1`: Pro-Government (895 comments) 
  - [cite_start]`-1`: Anti-Government (449 comments) 
  - [cite_start]`0`: Neutral (318 comments) 

## 🛠️ Tech Stack & Tools
- [cite_start]**Language:** Python 
- **Libraries:**
  - [cite_start]`scikit-learn` (Model building) 
  - [cite_start]`NLTK` (Natural Language Processing) 
  - [cite_start]`Pandas` (Data manipulation) 
  - [cite_start]`Matplotlib` / `Seaborn` (Data visualization) 
  - [cite_start]`youtube_comment_downloader` (Data collection) 
  - [cite_start]`google_trans` (Language translation) 

## ⚙️ Methodology
1.  **Data Collection:** Scraped comments from relevant political videos.
2.  [cite_start]**Translation:** Translated regional language comments to English for standardization.
3.  [cite_start]**Preprocessing:** Removed URLs, punctuation, and stopwords; applied lemmatization.
4.  [cite_start]**Feature Extraction:** Used **TF-IDF** (Term Frequency-Inverse Document Frequency) to convert text into numerical vectors.
5.  [cite_start]**Model Training:** Trained a **Logistic Regression** classifier on the processed data.

## 📈 Results
The model achieved robust performance across all sentiment classes:
- [cite_start]**Accuracy:** **94%** 
- [cite_start]**Macro F1-Score:** 0.94 
- [cite_start]**Key Observation:** The model showed high recall (98%) for pro-government comments, effectively capturing the dominant sentiment in the dataset.

## 🚀 Future Scope
- [cite_start]**Multilingual Support:** Native processing of regional languages without translation.
- [cite_start]**Real-Time Dashboard:** A visual interface for monitoring live sentiment trends.
- [cite_start]**Emotion Detection:** Extending analysis to detect specific emotions like anger, joy, or sarcasm.

## 👥 Author
- [cite_start]**Mohd Zaid** 

## 🙏 Acknowledgements
Special thanks to **Dr. [cite_start]Apurbalal Senapati** for guidance and support throughout this project.
