# Plant Thriving Predictor

![Python](https://img.shields.io/badge/Python-3.10%2B-blue?style=flat-square&logo=python)
![scikit-learn](https://img.shields.io/badge/scikit--learn-ML-orange?style=flat-square&logo=scikitlearn)
![Gradio](https://img.shields.io/badge/Gradio-UI-yellow?style=flat-square&logo=gradio)
![Jupyter](https://img.shields.io/badge/Jupyter-Notebook-F37626?style=flat-square&logo=jupyter)
![License](https://img.shields.io/badge/License-MIT-green?style=flat-square)
![Views](https://visitor-badge.laobi.icu/badge?page_id=Mordekai66.plant-thriving-predictor)

Binary classification pipeline that predicts whether a plant will thrive given environmental conditions. Trains and compares Logistic Regression and Decision Tree classifiers, tunes hyperparameters via GridSearchCV, and exposes a Gradio interface for real-time inference.

---

## Features

- Preprocessing: missing value removal, `LabelEncoder` for categorical columns, `StandardScaler` for numeric features
- Model comparison: Logistic Regression vs. Decision Tree (Accuracy, Precision, Recall, F1)
- Hyperparameter tuning via `GridSearchCV` with 5-fold cross-validation
- Confusion matrix visualization with Seaborn
- Interactive Gradio UI for live predictions

---

## Dataset

File: `plants_dataset_euhm_itai_07.csv`

| Feature | Type |
|---|---|
| Soil Type | Categorical — Sandy, Loamy, Clay |
| Sunlight (hours/day) | Numeric |
| Water Supply (liters/week) | Numeric |
| Temperature (C) | Numeric |
| pH Level | Numeric |
| Plant Species | Categorical — Fern, Rose, Cactus |
| **Thrives** | **Target — 0 / 1** |

---

## Setup

```bash
pip install -r requirements.txt
```

Place `plants_dataset_euhm_itai_07.csv` in the same directory as the notebook, then run all cells.

---

## Gradio Interface

After running the final cell, a local web UI launches. Select soil type and plant species from dropdowns, enter numeric values, and the model returns whether the plant will thrive under those conditions.

---

## Project Structure

```
.
├── plant thriving predictor.ipynb
├── plants_dataset_euhm_itai_07.csv
├── LICENSE
├── .gitignore
├── requirements.txt
└── README.md
```

---

