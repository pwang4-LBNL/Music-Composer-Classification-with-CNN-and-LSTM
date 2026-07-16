# Music-Composer-Classification-with-CNN-and-LSTM
This project develops and compares **Convolutional Neural Networks (CNN)** and **Long Short-Term Memory (LSTM)** models for automatic classical music composer classification using MIDI files. The study focuses on four composers: Bach, Beethoven, Chopin, and Mozart.

## Overview

This project develops and compares **Convolutional Neural Networks (CNN)** and **Long Short-Term Memory (LSTM)** models for classifying classical music composers using **MIDI** files.

The classification task focuses on four composers:

- Johann Sebastian Bach
- Ludwig van Beethoven
- Frédéric Chopin
- Wolfgang Amadeus Mozart

The project includes data preprocessing, exploratory data analysis (EDA), feature extraction, deep learning model development, and performance evaluation.

---

## Objectives

- Explore and analyze a MIDI dataset using exploratory data analysis (EDA).
- Preprocess MIDI files into machine learning representations.
- Develop CNN and LSTM models for composer classification.
- Compare the performance of both models.
- Evaluate classification accuracy and other performance metrics.

---

## Dataset

The dataset is provided as part of the course materials (Module 7).

Only the following four composers are included:

- Bach
- Beethoven
- Chopin
- Mozart

If additional MIDI files are used to address class imbalance, they are collected from publicly available datasets and properly cited in the final report.

---

## Workflow

```
MIDI Files
      │
      ▼
Data Cleaning
      │
      ▼
Exploratory Data Analysis (EDA)
      │
      ▼
Feature Extraction
      │
      ├──────────────┐
      ▼              ▼
 CNN Model      LSTM Model
      │              │
      ▼              ▼
Composer Prediction
      │
      ▼
Performance Comparison
```

---

## Repository Structure

```
music-composer-classification/
│
├── data/
│   ├── raw/
│   └── processed/
│
├── notebooks/
│   ├── EDA.ipynb
│   ├── CNN_Model.ipynb
│   └── LSTM_Model.ipynb
│
├── src/
│   ├── preprocessing.py
│   ├── feature_extraction.py
│   ├── cnn_model.py
│   ├── lstm_model.py
│   ├── train.py
│   └── evaluate.py
│
├── figures/
│
├── results/
│
├── README.md
└── requirements.txt
```

---

## Exploratory Data Analysis

The EDA includes:

- Composer distribution
- Class balance
- MIDI sequence length distribution
- Pitch distribution
- Note duration distribution
- Tempo distribution
- Piano roll visualization
- Basic MIDI statistics

---

## Models

### CNN

The CNN model learns local musical patterns from MIDI representations such as piano rolls or feature matrices.

### LSTM

The LSTM model learns temporal dependencies from sequential note events in MIDI files.

---

## Evaluation Metrics

The following metrics are used to evaluate model performance:

- Accuracy
- Precision
- Recall
- F1-score
- Confusion Matrix

---

## Technologies

- Python
- PyTorch
- NumPy
- Pandas
- Matplotlib
- pretty_midi
- music21
- scikit-learn

---

## Installation

Clone the repository:

```bash
git clone https://github.com/your_username/music-composer-classification.git
cd music-composer-classification
```

Install dependencies:

```bash
pip install -r requirements.txt
```

---

## Running the Project

Run data preprocessing:

```bash
python src/preprocessing.py
```

Train the CNN model:

```bash
python src/train.py --model cnn
```

Train the LSTM model:

```bash
python src/train.py --model lstm
```

Evaluate the model:

```bash
python src/evaluate.py
```

---

## Results

The final report compares CNN and LSTM performance for composer classification and discusses the strengths and limitations of each architecture.

---

## Contributors

- Peng Wang
- April
- Akua

University of San Diego

Applied Artificial Intelligence

---

## License

This project is for educational purposes only.
