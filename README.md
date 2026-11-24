# Week 2 NLP Text Classification Final

This project predicts whether an SMS message is **ham (normal)** or **spam** using machine-learning classifiers.

## What it does
- Retrieves the UCI SMS Spam Collection dataset if the raw file is not already present.
- Cleans the data (missing entries, duplicate rows, labels, and blank text).
- Uses TF-IDF features with unigram and bigram terms.
- Trains and compares Multinomial Naive Bayes and Linear SVM.
- Reports accuracy, spam precision, spam recall, and spam F1.
- Saves confusion-matrix charts, a comparison CSV, a run summary, and the best model.

## Project layout
```text
Week2-NLP-Text-Classification-Final/
├── README.md
├── requirements.txt
├── .gitignore
├── src/
│   └── train_classifier.py
├── data/
├── models/
└── reports/
```

## Setup
Run from the project's root directory:
```bash
python -m pip install -r requirements.txt
```

## Run
```bash
python src/train_classifier.py
```
The first run needs an internet connection to download the dataset from UCI. Generated files are written into `data/`, `models/`, and `reports/`.

## Models and selection
- Multinomial Naive Bayes
- Linear Support Vector Machine (Linear SVM)

The script selects the best model based on the spam F1-score.

## Dataset
SMS Spam Collection, UCI Machine Learning Repository.
