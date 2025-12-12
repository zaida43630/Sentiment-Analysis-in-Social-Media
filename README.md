# Political Sentiment Analysis in Social Media

## 📌 Project Overview
This project aims to automate the analysis of public opinion trends by classifying YouTube comments into political sentiment categories. Using Natural Language Processing (NLP) and Machine Learning techniques, the system interprets user-generated content to gauge public sentiment towards the government.

## 🎯 Objectives
- **Sentiment Classification:** Categorize comments into **Pro-Government**, **Anti-Government**, or **Neutral**.
- **Data Processing:** Collect, clean, and preprocess raw user-generated text.
- **Trend Analysis:** Identify public opinion trends regarding government policies.

## 📊 Dataset
- **Source:** Comments collected from videos of prominent political influencers on YouTube.
- **Size:** 1,664 comments.
- **Labeling:** Manually labeled into three classes:
  - `1`: Pro-Government (895 comments) 
  - `-1`: Anti-Government (449 comments) 
  - `0`: Neutral (318 comments) 

## 🛠️ Tech Stack & Tools
- **Language:** Python 
- **Libraries:**
  - `scikit-learn` (Model building) 
  - `NLTK` (Natural Language Processing) 
  - `Pandas` (Data manipulation) 
  - `Matplotlib` / `Seaborn` (Data visualization) 
  - `youtube_comment_downloader` (Data collection) 
  - `google_trans` (Language translation) 

## ⚙️ Methodology
1.  **Data Collection:** Scraped comments from relevant political videos.
2.  **Translation:** Translated regional language comments to English for standardization.
3.  **Preprocessing:** Removed URLs, punctuation, and stopwords; applied lemmatization.
4.  **Feature Extraction:** Used **TF-IDF** (Term Frequency-Inverse Document Frequency) to convert text into numerical vectors.
5.  **Model Training:** Trained a **Logistic Regression** classifier on the processed data.

## 📈 Results
The model achieved robust performance across all sentiment classes:
- **Accuracy:** **94%** 
- **Macro F1-Score:** 0.94 
- **Key Observation:** The model showed high recall (98%) for pro-government comments, effectively capturing the dominant sentiment in the dataset.

## 🚀 Future Scope
- **Multilingual Support:** Native processing of regional languages without translation.
- **Real-Time Dashboard:** A visual interface for monitoring live sentiment trends.
- **Emotion Detection:** Extending analysis to detect specific emotions like anger, joy, or sarcasm.

## 👥 Author
- **Mohd Zaid** 
