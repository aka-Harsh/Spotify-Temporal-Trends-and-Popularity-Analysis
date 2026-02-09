# Spotify Music Popularity Prediction

A comprehensive machine learning analysis investigating what drives music success on Spotify's Global Top 200 charts (2017-2023). This project explores temporal streaming patterns and compares the predictive power of audio features versus artist reputation in determining track popularity.

## Libraries & Packages Used

- pandas
- numpy
- matplotlib
- seaborn
- tqdm
- sklearn
- XGBoost 
- os


## Installation & Setup

You can either install the required packages globally or create a virtual environment inside this project directory. To set up the virtual environment, run:

```bash
python -m venv venv 
venv\Scripts\activate
pip install -r requirements.txt
```

After completing the setup, open the notebooks **main.ipynb** and **Temporal Analysis.ipynb**. Running all cells in these notebooks will generate the following:

1. ***Main***
- Built artist history and time-aware features 
- Conducted EDA with univariate histograms, bivariate boxplots by target class, and a correlation heatmap.
- Model development and performance comparison with alternative models.
- Generated confusion matrices and classification reports for the best combined models, along with per-class metrics.

2. ***Temporal analysis***
- Streaming pattern (Yearly, Monthly, and Weekly)
- Longitivity of the songs (Yearly)
- Collabration trend (Yearly) 

## Key Findings

1. Artist reputation features consistently outperform audio features in predicting song success
2. XGBoost achieved the highest accuracy (~70%) across all feature configurations
3. Song chart longevity decreased by 56% from 2017 to 2022 (73 days → 32 days)
4. Weekend streaming peaks at +2.2% above weekday average (Saturday highest)
5. COVID-19 pandemic caused a 7.8% drop in streaming points and reduced collaborations

## Technical Details

**Algorithms Used:**
- Random Forest
- Logistic Regression
- XGBoost
- Support Vector Machine (SVM)

**Feature Engineering:**
- Audio features: Danceability, Energy, Loudness, Speechiness, Acousticness, Instrumentalness, Valence
- Artist features: Historical performance, experience, release frequency, collaboration metrics
- Time-aware aggregation for artist reputation tracking

## Contributors

- Govind Saraswat
- Lisha 
- Sarthak

*MSc Data Science, University of Edinburgh*
