# 🎥 IMDb Movie Review Sentiment Analysis

## 📌 Project Overview
This project aims to build a machine learning model that classifies IMDb movie reviews as **positive** or **negative**. The dataset consists of 50,000 reviews with equal distribution. Using text preprocessing, feature engineering, and machine learning techniques, the project strives to achieve a high-performing sentiment classification model.

## 🚀 Problem Statement
The primary objective is to predict the sentiment of IMDb movie reviews. The dataset contains reviews labeled as either positive or negative. Through preprocessing, feature extraction (like TF-IDF), and classification algorithms, we aim to build an optimized sentiment analysis model.

## 📂 Dataset
- **Size**: 50,000 reviews
- **Labels**: Balanced between positive (25,000) and negative (25,000)
- **Columns**:
  - `review`: The textual content of the movie review
  - `sentiment`: The sentiment label (positive or negative)

## 🔎 Data Exploration
- Visualized class distribution (balanced dataset)
- Plotted review length distribution to understand text characteristics

## 🔄 Data Preprocessing
- Removed HTML tags and non-alphabetic characters
- Converted text to lowercase
- Tokenized the reviews
- Removed stopwords
- Applied lemmatization

The output was stored in a new column `clean_review` for further analysis.

## 🛠️ Feature Engineering
- Computed the following features:
  - **Word Count**
  - **Character Count**
  - **Average Word Length**
- Applied **TF-IDF Vectorization** to transform text into numerical features with a maximum of 5000 features.

## 🤖 Model Development & Evaluation
| Model               | 🎯 Train Accuracy | 🚀 Test Accuracy | 📊 F1-Score | 💡 Comments                       |
|----------------------|------------------|-----------------|-------------|---------------------------------|
| **Logistic Regression** | 92.3%          | 88.7%          | 89%         | Best performer with optimal F1-score |
| **LSTM**               | N/A            | 88.4%          | 88%         | Deep learning model with strong performance |
| **SVM (LinearSVC)**    | 92.9%          | 88.2%          | 88%         | Competitive accuracy                     |
| **Random Forest**      | 88.6%          | 82.9%          | 83%         | Lowest among tested models              |

**Final Model Choice**: Logistic Regression was selected for future predictions due to its balance of performance and simplicity.

## 📊 Visualization
- **Word Clouds**:
  - Positive Reviews: Clean, hopeful, emotional terms.
  - Negative Reviews: Critical, disappointed tone.

## 🔮 Predicting Future Sentiments
- A custom function was developed for real-time sentiment prediction using the trained Logistic Regression model and TF-IDF vectorization.

## 💡 Insights
1. Logistic Regression outperformed other models in terms of accuracy and F1-score.
2. Deep learning with LSTM was competitive, suggesting potential with further optimization.
3. Feature engineering with TF-IDF effectively represented textual data for model training.
4. Visualizations helped understand the common terms in positive and negative sentiments.

## 🔭 Future Work
- Explore advanced models like BERT for better sentiment understanding.
- Optimize LSTM with more epochs and hyperparameter tuning.
- Implement model interpretability techniques.

## 🎬 Video Explanation
[▶️ Video Walkthrough](https://drive.google.com/file/d/1nw_0co-exFVrcuq8I-XDfWX-QMBBm3tF/view?usp=sharing)

---

Feel free to contribute to this project or raise issues for improvements.

### 👨‍💻 Author
**P Rohith Raveendran**
