# Data Preprocessing

Learn the basics of cleaning and preparing data before modeling.

What you'll learn
- Inspect missing values
- Fill, forward/backward fill, and interpolate
- Basic visualization of missingness

Hands-on notebook
- Open: notebooks/data-cleaning.ipynb
- Data used: data/Iris for cleaning.csv

Key steps covered
- df.isnull().sum(), heatmaps of missingness
- Strategies: dropna, fillna(0), ffill, bfill, interpolate

Tips
- Keep a copy of raw data
- Track which columns are imputed

Next steps
- Move to classification with Iris: docs/classification.md
- Or read more: docs/regularization-and-overfitting.md
