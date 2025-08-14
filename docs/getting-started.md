# Getting Started

Goal: set up your environment and run your first notebooks in this repo.

What you'll learn
- Install Python and Jupyter
- Open and run notebooks
- Understand the repository layout

Prerequisites
- Python 3.9+ (3.10+ recommended)
- pip or conda

Quick setup (pip)
1) Create a virtual environment
   - macOS/Linux: `python3 -m venv .venv && source .venv/bin/activate`
2) Install basics: `pip install -U jupyter numpy pandas seaborn scikit-learn matplotlib`
3) Start Jupyter: `jupyter notebook`

First notebooks
- Intro to Jupyter: notebooks/intro.ipynb
- Data cleaning (Iris): notebooks/data-cleaning.ipynb
- Classification on Iris: notebooks/iris-data-for-beginners.ipynb

Datasets
- Small CSVs live in data/
- Iris dataset: data/Iris.csv
- Iris (with missing values for cleaning practice): data/Iris for cleaning.csv

Next steps
- Continue to: docs/data-preprocessing.md
- Or jump to: docs/classification.md
