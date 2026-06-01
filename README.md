# Comment Category Prediction

## Overview

This repository contains my solution for the Kaggle **Comment Category Prediction Challenge**.

The objective is to predict the final category assigned to a user comment using textual information, metadata, interaction statistics, and platform-generated indicators.

---

## Dataset

The dataset consists of:

- **train.csv** - Training data with labeled comments
- **test.csv** - Test data for predictions
- **sample_submission.csv** - Sample submission format

### Features

| Feature | Description |
|---------|-------------|
| comment | Raw comment text |
| created_date | Timestamp |
| post_id | Post identifier |
| emoticon_1 | Emoticon group 1 |
| emoticon_2 | Emoticon group 2 |
| emoticon_3 | Emoticon group 3 |
| upvote | Positive reactions |
| downvote | Negative reactions |
| if_1 | Internal hidden feature |
| if_2 | Internal hidden feature |
| race | Identity indicator |
| religion | Topic indicator |
| gender | Topic indicator |
| disability | Topic indicator |

**Target Variable:** `label` (four categories)

---

## Project Structure

```
Comment-Category-Prediction/
│
├── data/
│   ├── train.csv
│   ├── test.csv
│   └── sample_submission.csv
│
├── notebooks/
│   └── 23f3001921-notebook-t12026.ipynb
│
├── outputs/
│   └── submission.csv
│
├── requirements.txt
├── README.md
└── .gitignore
```

---

## Methodology

### 1. Data Exploration
- Dataset inspection
- Missing value analysis
- Feature type analysis
- Target distribution analysis

### 2. Data Preprocessing
- Missing value handling
- Date feature extraction
- Text cleaning
- Feature encoding

### 3. Feature Engineering
- TF-IDF text representation
- Metadata features
- Numerical feature scaling

### 4. Model Training

Models explored:
- Logistic Regression
- Random Forest
- XGBoost
- LightGBM

### 5. Evaluation

Competition metric used for leaderboard evaluation.

---

## Results

### Best Public Leaderboard Score

**0.81690**

---

## Running Locally

Clone repository:

```bash
git clone https://github.com/ShreyaThakur05/Comment_Category_Prediction.git
cd Comment-Category-Prediction
```

Install dependencies:

```bash
pip install -r requirements.txt
```

Run notebook:

```bash
jupyter notebook
```

Then open `notebooks/23f3001921-notebook-t12026.ipynb`

---

## Submission File

Final predictions are available in:

```
outputs/submission.csv
```

---

## Author

**Shreya Thakur**

---

