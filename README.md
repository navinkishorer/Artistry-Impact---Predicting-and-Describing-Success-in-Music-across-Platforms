# 🎵 Artistry Impact: Predicting and Describing Success in Music Across Platforms

## 📌 Overview

This project explores the factors that influence the popularity of songs using data from Spotify and YouTube. Using a blend of clustering, logistic regression, and neural networks, we attempt to predict which features make a song successful and assess if older tracks could trend today.

---

## 👨‍🎓 Project Info

- **Course**: BAN 620 – Data Mining  
- **Semester**: Fall 2023  
- **Team Name**: Group 1  
- **Contributors**:  
  - Harshini Jawahar  
  - Navin Kishore Ravi Kumar  
  - Pranav Hegde  
  - Prasad Dattatraya Pilankar  
  - Rishab Reddy Bandi  

---

## 🎯 Objective

To identify which audio and metadata attributes most strongly predict a song’s popularity and to evaluate whether past hits could still gain traction in the current digital music landscape.

---

## 📂 Dataset

- **Source**: Kaggle  
- **Title**: Spotify and YouTube - Statistics for the Top 10 Songs of Various Artists  
- **Size**: ~20,000 songs by 2079 artists  
- **Platforms**: Spotify & YouTube  
- **Timeframe**: Data collected until February 7, 2023

---

## 🧪 Methodology

### 1. Data Preprocessing
- Removed ~400 rows with missing values.
- Encoded special characters to ensure compatibility.
- Dropped non-essential columns (e.g., URLs, indexes, descriptions).
- Segregated a few hand-picked "old songs" for retrospective popularity analysis.

### 2. Exploratory Data Analysis (EDA)
- Correlation heatmaps
- Distribution visualizations
- Cluster profiling

### 3. Clustering (KMeans)
- Grouped songs into 6 clusters based on views, likes, and acoustic features.
- Consolidated them into 3 popularity tiers: **low**, **medium**, and **high**.

### 4. Predictive Modeling
- **Logistic Regression**: Provided interpretability and quick inference.
- **Neural Network**: 2 hidden layers (64 and 32 nodes), 1000 iterations, adaptive learning.

### 5. Evaluation
- Compared performance of models based on accuracy and classification metrics.
- Assessed model generalizability using test sets and old songs.

---

## 📈 Key Findings

- **Best Predictors**: `danceability` and `loudness` had the strongest association with popularity.
- **Model Choice**: Neural Networks outperformed logistic regression in identifying popular songs, especially on edge cases.
- **Old Song Revival**: Tracks like *Smooth Criminal*, *Dear Mama*, and *Iron Man* were predicted to still be popular in today's climate.

---

## 💡 Recommendations

### For Spotify:
- Consider remastering and promoting older tracks that fit today's successful feature profile.
- Use popularity predictors like `danceability` for seasonal song promotions (e.g., weddings, festivals).

### For Music Producers:
- Focus on optimizing key features (danceability, loudness, valence) that align with popular trends.
- Balance production values with experimental or unique sound elements to stand out.

---

## 📁 Repository Structure

```bash
.
├── Refactored_Final_code.ipynb   # Cleaned and well-commented notebook
├── README.md                     # Project overview and documentation
├── old_songs_predictions.csv     # Neural Net predictions for old songs
├── visualizations/               # EDA and clustering plots
└── data/                         # Processed dataset used in this project
